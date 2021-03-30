---
title: Kurumsal Uygulamaların listesini al
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
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405509"
---
# <a name="get-a-list-of-enterprise-applications"></a>Kurumsal Uygulamaların listesini al

1. Powershell **komutu aracılığıyla** kurumsal uygulamaların (tüm uygulamalar veya Görünen ad, Kimlik, Tanımlayıcı URL'ler vb. ile filtrelenmiş) listesini almak için bkz. [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Powershell komutu aracılığıyla hizmet asıl nesnelerinin (tüm nesneler veya kimlikle filtrelenmiş) listesini almak için bkz. [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. SAML yapılandırılmış uygulamalarının listesini almak için **aşağıdaki PowerShell betikleri size** yardımcı olabilir:

    Her Uygulama bir OAuth uygulaması veya SAML uygulaması (hem galeri hem de galeri olmayan uygulamalar) kayıt işlemi sırasında AAD'de oluşturulmuş iki nesne olabilir. Bunlardan biri Uygulama Nesnesi, diğeri de Hizmet Sorumlusu nesnesidir. PowerShell kullanarak Hizmet Asıl Nesnesinin özelliklerini dökümü ederken, her uygulamanın aşağıdaki gibi ilişkili belirli sayıda Etiketi olduğunu bulursanız:

    - OAuth uygulamalarının **"WindowsAzureActiveDirectoryIntegratedApp**" adlı bir etiketi olabilir
    - Galeri SAML Uygulamaları'nın **"WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**" adlı bir etiketi olabilir
    - Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Bu nedenle, bu etiketleri kullanabilir ve ne tür bir uygulama olduğunu bulabilirsiniz. **"WindowsAzureActiveDirectoryIntegratedApp**" etiketi, tüm uygulama türleri için yaygındır. Tüm SAML uygulamalarını (galeri hem de galeri dışı) listeleyen aşağıdaki parçacığı kullanabilirsiniz:

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Daha fazla bilgi için [Bkz. Azure AD'de SAML özellikli uygulamaları tanımlama.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Yalnızca Web uygulamalarını bulma ve listele:**"Web app/API" uygulama türüne sahip tüm Azure AD uygulamalarını almak için aşağıdaki komutu kullanın

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. Tek başına Yerel uygulamaları bulun ve **listele:** Tüm yerel istemci (masaüstü/mobil cihaz) uygulamalarını almak için aşağıdaki komutu çalıştırın.

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Tüm Kayıtlı Azure AD Uygulama Ayrıntılarını CSV olarak** dışarı aktar : Aşağıdaki komut, gerekli ayrıntıların bulunduğu tüm Azure AD uygulamalarını csv dosyasına dışarı aktarır:

    - Get-AzureADApplication -All:$true | Select-Object Adı, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Kullanılmayan Azure uygulamalarının listesini dışarı aktarmanız gerekiyor** – Denetim raporu

    Azure AD Premium lisansına sahip olmak şartıyla, Azure AD yalnızca 30 gün boyunca uygulama günlüklerini gösterebilir.
    Verileri 30 gün daha uzun süre tutmak için iki seçeneğiniz vardır. Verileri programatik [olarak almak ve veritabanında](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) depolamak için Azure AD Raporlama API'lerini kullanabilirsiniz. Alternatif olarak, denetim günlüklerini üçüncü taraf SIEM sistemiyle tümleştirebilirsiniz.

    Ayrıca, Azure Active Directory>Uygulama Kayıtları altında tüm uygulamalara ve sahip olunan uygulamalara ait uygulama listesini>Tüm uygulamalara/Sahip>uygulamaları indirebilirsiniz.

    MS Graph aracılığıyla uygulamaların listesini almak için Liste uygulamaları [- Microsoft Graph v1.0 ve](https://docs.microsoft.com/graph/api/application-list) uygulama kaynak türü - Microsoft Graph [v1.0](https://docs.microsoft.com/graph/api/resources/application)'a bakın.
