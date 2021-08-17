---
title: Enterprise Uygulamalarının listesini al
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116748"
---
# <a name="get-a-list-of-enterprise-applications"></a>Enterprise Uygulamalarının listesini al

1. Powershell **komutu aracılığıyla** kurumsal uygulamaların (tüm uygulamalar veya Görünen ad, Kimlik, Tanımlayıcı URL'ler vb. olarak filtrelenmiş) listesini almak için bkz. [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Powershell komutu aracılığıyla hizmet asıl nesnelerinin (tüm nesneler veya kimlikle filtrelenmiş) listesini almak için bkz. [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. SAML yapılandırılmış **uygulamalarının listesini almak için, aşağıdaki PowerShell betikleri size** yardımcı olabilir:

    Her Uygulama bir OAuth uygulaması veya SAML uygulaması (hem galeri hem de galeri olmayan uygulamalar) kayıt işlemi sırasında AAD'de oluşturulmuş iki nesne olabilir. Bunlardan biri Uygulama Nesnesi, diğeri ise Hizmet Sorumlusu nesnesidir. PowerShell kullanarak Hizmet Sorumlusu Nesnesi'nin özelliklerini dökümü 10.000'e bırakarak, her uygulamanın belirli sayıda Etiketi olduğunu ve bunun gibi ilişkili olduğunu bulursanız:

    - OAuth uygulamalarının "**WindowsAzureActiveDirectoryIntegratedApp**" adlı bir etiketi olabilir
    - Galeri SAML Apps, "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**" adlı bir etikete sahip olabilir
    - Non-Gallery SAML Apps would a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Bu nedenle, bu etiketleri kullanabilir ve ne tür bir uygulama olduğunu bulabilirsiniz. "**WindowsAzureActiveDirectoryIntegratedApp**" etiketi, tüm uygulama türlerinde yaygındır. Tüm SAML uygulamalarını (hem galeri hem de galeri dışı) listeleyen aşağıdaki parçacıkyı kullanabilirsiniz:

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Daha fazla bilgi için [bkz. Azure AD'de SAML etkinleştirilmiş uygulamaları tanımlama.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Yalnızca Web uygulamalarını bulma ve listele:**"Web uygulaması/API" uygulama türüyle tüm Azure AD uygulamalarını almak için aşağıdaki komutu kullanın

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Tek başına Yerel uygulamaları bulma** ve listele: Tüm yerel istemci (masaüstü/mobil cihaz) uygulamalarını almak için aşağıdaki komutu çalıştırın.

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Tüm Kayıtlı Azure AD Uygulama Ayrıntılarını CSV'ye** Aktar : Aşağıdaki komut, gerekli ayrıntıların bulunduğu tüm Azure AD uygulamalarını csv dosyasına dışarı aktarır:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Kullanılmayan Azure uygulamalarının listesini dışarı aktarmanız gerekiyor** – Denetim raporu

    Azure AD, lisans sahibi olmak şartıyla, uygulama günlüklerini yalnızca 30 Azure AD Premium gösterebilir.
    Verileri 30 gün daha uzun süre tutmak için iki seçeneğiniz vardır. Verileri programatik [olarak almak ve veritabanında](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) depolamak için Azure AD Raporlama API'lerini kullanabilirsiniz. Alternatif olarak, denetim günlüklerini üçüncü taraf SIEM sistemiyle tümleştirebilirsiniz.

    Ayrıca, Azure Active Directory altında tüm uygulamalara ve sahip olunan uygulamalara ait uygulama listesini indirebilirsiniz>Kayıtları>Tüm uygulamalar>Sahip olunan uygulamaları indirin.

    MS Graph aracılığıyla uygulama listesini almak için bkz. Liste uygulamaları [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) ve uygulama kaynak [türü - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
