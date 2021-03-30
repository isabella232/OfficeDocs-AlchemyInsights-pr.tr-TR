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
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="a72ac-102">Kurumsal Uygulamaların listesini al</span><span class="sxs-lookup"><span data-stu-id="a72ac-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="a72ac-103">Powershell **komutu aracılığıyla** kurumsal uygulamaların (tüm uygulamalar veya Görünen ad, Kimlik, Tanımlayıcı URL'ler vb. ile filtrelenmiş) listesini almak için bkz. [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span><span class="sxs-lookup"><span data-stu-id="a72ac-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="a72ac-104">Powershell komutu aracılığıyla hizmet asıl nesnelerinin (tüm nesneler veya kimlikle filtrelenmiş) listesini almak için bkz. [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="a72ac-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="a72ac-105">SAML yapılandırılmış uygulamalarının listesini almak için **aşağıdaki PowerShell betikleri size** yardımcı olabilir:</span><span class="sxs-lookup"><span data-stu-id="a72ac-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="a72ac-106">Her Uygulama bir OAuth uygulaması veya SAML uygulaması (hem galeri hem de galeri olmayan uygulamalar) kayıt işlemi sırasında AAD'de oluşturulmuş iki nesne olabilir.</span><span class="sxs-lookup"><span data-stu-id="a72ac-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="a72ac-107">Bunlardan biri Uygulama Nesnesi, diğeri de Hizmet Sorumlusu nesnesidir.</span><span class="sxs-lookup"><span data-stu-id="a72ac-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="a72ac-108">PowerShell kullanarak Hizmet Asıl Nesnesinin özelliklerini dökümü ederken, her uygulamanın aşağıdaki gibi ilişkili belirli sayıda Etiketi olduğunu bulursanız:</span><span class="sxs-lookup"><span data-stu-id="a72ac-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="a72ac-109">OAuth uygulamalarının **"WindowsAzureActiveDirectoryIntegratedApp**" adlı bir etiketi olabilir</span><span class="sxs-lookup"><span data-stu-id="a72ac-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="a72ac-110">Galeri SAML Uygulamaları'nın **"WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**" adlı bir etiketi olabilir</span><span class="sxs-lookup"><span data-stu-id="a72ac-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="a72ac-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="a72ac-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="a72ac-112">Bu nedenle, bu etiketleri kullanabilir ve ne tür bir uygulama olduğunu bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a72ac-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="a72ac-113">**"WindowsAzureActiveDirectoryIntegratedApp**" etiketi, tüm uygulama türleri için yaygındır.</span><span class="sxs-lookup"><span data-stu-id="a72ac-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="a72ac-114">Tüm SAML uygulamalarını (galeri hem de galeri dışı) listeleyen aşağıdaki parçacığı kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="a72ac-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="a72ac-115">Daha fazla bilgi için [Bkz. Azure AD'de SAML özellikli uygulamaları tanımlama.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="a72ac-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="a72ac-116">**Yalnızca Web uygulamalarını bulma ve listele:**"Web app/API" uygulama türüne sahip tüm Azure AD uygulamalarını almak için aşağıdaki komutu kullanın</span><span class="sxs-lookup"><span data-stu-id="a72ac-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="a72ac-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="a72ac-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="a72ac-118">Tek başına Yerel uygulamaları bulun ve **listele:** Tüm yerel istemci (masaüstü/mobil cihaz) uygulamalarını almak için aşağıdaki komutu çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="a72ac-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="a72ac-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="a72ac-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="a72ac-120">**Tüm Kayıtlı Azure AD Uygulama Ayrıntılarını CSV olarak** dışarı aktar : Aşağıdaki komut, gerekli ayrıntıların bulunduğu tüm Azure AD uygulamalarını csv dosyasına dışarı aktarır:</span><span class="sxs-lookup"><span data-stu-id="a72ac-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="a72ac-121">Get-AzureADApplication -All:$true | Select-Object Adı, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="a72ac-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="a72ac-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="a72ac-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="a72ac-123">**Kullanılmayan Azure uygulamalarının listesini dışarı aktarmanız gerekiyor** – Denetim raporu</span><span class="sxs-lookup"><span data-stu-id="a72ac-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="a72ac-124">Azure AD Premium lisansına sahip olmak şartıyla, Azure AD yalnızca 30 gün boyunca uygulama günlüklerini gösterebilir.</span><span class="sxs-lookup"><span data-stu-id="a72ac-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="a72ac-125">Verileri 30 gün daha uzun süre tutmak için iki seçeneğiniz vardır.</span><span class="sxs-lookup"><span data-stu-id="a72ac-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="a72ac-126">Verileri programatik [olarak almak ve veritabanında](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) depolamak için Azure AD Raporlama API'lerini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a72ac-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="a72ac-127">Alternatif olarak, denetim günlüklerini üçüncü taraf SIEM sistemiyle tümleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a72ac-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="a72ac-128">Ayrıca, Azure Active Directory>Uygulama Kayıtları altında tüm uygulamalara ve sahip olunan uygulamalara ait uygulama listesini>Tüm uygulamalara/Sahip>uygulamaları indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a72ac-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="a72ac-129">MS Graph aracılığıyla uygulamaların listesini almak için Liste uygulamaları [- Microsoft Graph v1.0 ve](https://docs.microsoft.com/graph/api/application-list) uygulama kaynak türü - Microsoft Graph [v1.0](https://docs.microsoft.com/graph/api/resources/application)'a bakın.</span><span class="sxs-lookup"><span data-stu-id="a72ac-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
