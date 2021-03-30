---
title: Uygulama Kayıt Sahibi sorunları
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
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405324"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="a7158-102">Uygulama Kayıt Sahibi sorunları</span><span class="sxs-lookup"><span data-stu-id="a7158-102">App Registration Owner issues</span></span>

<span data-ttu-id="a7158-103">Aşağıda, uygulama kayıtlarda sorumluları sahip olarak eklemenin kullanılabilir yöntemleri yer almaktadır:</span><span class="sxs-lookup"><span data-stu-id="a7158-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="a7158-104">Azure AD PowerShell Modülünü Kullanma -</span><span class="sxs-lookup"><span data-stu-id="a7158-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="a7158-105">Başvuru: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="a7158-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="a7158-106">Azure CLI kullanma - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="a7158-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="a7158-107">Başvuru: [az reklam uygulaması sahibi](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="a7158-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="a7158-108">MS Graph'i kullanma -</span><span class="sxs-lookup"><span data-stu-id="a7158-108">Using MS Graph -</span></span>

    <span data-ttu-id="a7158-109">Başvuru: [Sahip ekleme - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="a7158-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="a7158-110">Azure AD Portalını kullanma - Portal.azure.com [>](https://portal.azure.com/) Azure Active directory > Uygulama Kaydı'> > Sahipler > Ekle'yi seçin</span><span class="sxs-lookup"><span data-stu-id="a7158-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="a7158-111">**Uygulamanın sahibi sizseniz bile uygulama kayıtlarda görüntülene misiniz?**</span><span class="sxs-lookup"><span data-stu-id="a7158-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="a7158-112">Uygulamanın sahibi yönetim rolü değildir.</span><span class="sxs-lookup"><span data-stu-id="a7158-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="a7158-113">[Azure AD yönetim portalına](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) erişimi kısıtla ayarı etkinleştirilirse, uygulama kayıt portalında uygulamaları yalnızca yönetici ilebilir.</span><span class="sxs-lookup"><span data-stu-id="a7158-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="a7158-114">Bir sahibin uygulamaları görüntüley olması için, bu ayarı devre dışı bırak (Bunu HAYıR olarak ayarla) veya yönetici rolünü yalnızca belirli bir uygulamanın sahibine attayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a7158-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="a7158-115">Ancak bunun için Azure AD Premium P2 lisansına sahip olmak ve Ayrıcalıklı Kimlik Yönetimi'yi [etkinleştirmek gerekir.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="a7158-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
