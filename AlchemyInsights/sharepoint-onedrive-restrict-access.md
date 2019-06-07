---
title: SharePoint veya OneDrive erişimi sınırlama
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 3227f10270148c0e515b687c48058affa4d2be70
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759100"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="6fcf9-102">SharePoint veya OneDrive erişimi sınırlama</span><span class="sxs-lookup"><span data-stu-id="6fcf9-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="6fcf9-103">SharePoint çevrimiçi/OneDrive hizmetlerine erişimi kısıtlamak için birçok yol vardır.</span><span class="sxs-lookup"><span data-stu-id="6fcf9-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="6fcf9-104">Bu çeşitli erişim kısıtlama yöntemleri aşağıda özetlenmiştir.</span><span class="sxs-lookup"><span data-stu-id="6fcf9-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="6fcf9-105">İzni kısıtlama</span><span class="sxs-lookup"><span data-stu-id="6fcf9-105">Permission Restriction</span></span>

<span data-ttu-id="6fcf9-106">SharePoint çevrimiçi ve iş OneDrive, biz siteleri, dosyalar ve klasörler gibi öğeleri erişimi olmalıdır bu gruplar/kişiler erişim vererek kısıtlayın.</span><span class="sxs-lookup"><span data-stu-id="6fcf9-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

[<span data-ttu-id="6fcf9-107">SharePoint liste veya kitaplık izinlerini Özelleştir</span><span class="sxs-lookup"><span data-stu-id="6fcf9-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[<span data-ttu-id="6fcf9-108">SharePoint site izinlerini özelleştirme</span><span class="sxs-lookup"><span data-stu-id="6fcf9-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

[<span data-ttu-id="6fcf9-109">Bir alt klasör izinlerini değiştirme</span><span class="sxs-lookup"><span data-stu-id="6fcf9-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[<span data-ttu-id="6fcf9-110">Yönetilmeyen cihazlardan erişimi denetleme</span><span class="sxs-lookup"><span data-stu-id="6fcf9-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="6fcf9-111">SharePoint veya Office 365'te genel yönetim bloke edebilir veya yönetilmeyen aygıtlardan SharePoint ve OneDrive içeriğe erişimi sınırlama (Bu karma AD birleştirilmiş veya Intune uyumlu).</span><span class="sxs-lookup"><span data-stu-id="6fcf9-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="6fcf9-112">Ağ konumu kısıtlama</span><span class="sxs-lookup"><span data-stu-id="6fcf9-112">Network Location Restriction</span></span>

<span data-ttu-id="6fcf9-113">Bir BT yöneticisi, güvendiğiniz tanımlanan ağ konumlarına dayalı SharePoint ve OneDrive kaynaklarına erişimi denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6fcf9-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="6fcf9-114">Konum temelli ilke olarak da budur.</span><span class="sxs-lookup"><span data-stu-id="6fcf9-114">This is also known as location-based policy.</span></span> <span data-ttu-id="6fcf9-115">Daha fazla bilgi için lütfen [SharePoint çevrimiçi ve ağ konumuna bağlı olarak OneDrive veri erişimi denetleme](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) bkz:</span><span class="sxs-lookup"><span data-stu-id="6fcf9-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="6fcf9-116">Site kilit kısıtlaması</span><span class="sxs-lookup"><span data-stu-id="6fcf9-116">Site Lock Restriction</span></span> 

<span data-ttu-id="6fcf9-117">SharePoint içinde çevrimiçi erişimi olan hiç kimse için bir site koleksiyonu kilitleme olanağı vardır.</span><span class="sxs-lookup"><span data-stu-id="6fcf9-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="6fcf9-118">Bu PowerShell ve [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState özelliğini kullanarak [SharePoint çevrimiçi Yönetimi Kabuk](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) aracılığıyla ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="6fcf9-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="6fcf9-119">Kullanıcıların site veya alt site oluşturmasını kısıtlamak</span><span class="sxs-lookup"><span data-stu-id="6fcf9-119">Restrict users from creating sites or subsites</span></span>

<span data-ttu-id="6fcf9-120">SharePoint Yönetim veya Office 365 genel yönetici, kullanıcılarınızın oluşturmak ve kendi SharePoint sitelerini yönetmek, bunlar ne tür siteler oluşturabilir, belirlemek sağlayabilirsiniz ve siteleri konumunu belirtin.</span><span class="sxs-lookup"><span data-stu-id="6fcf9-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="6fcf9-121">Daha fazla bilgi için lütfen bkz [Yönet Online'da SharePoint sitesi oluşturma](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="6fcf9-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

