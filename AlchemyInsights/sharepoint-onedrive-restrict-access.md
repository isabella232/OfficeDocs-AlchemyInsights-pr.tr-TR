---
title: SharePoint veya OneDrive'da erişimi kısıtlama
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750684"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="c2880-102">SharePoint veya OneDrive'da erişimi kısıtlama</span><span class="sxs-lookup"><span data-stu-id="c2880-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="c2880-103">SharePoint Online/OneDrive hizmetlerine erişimi kısıtlamanın birçok yolu vardır.</span><span class="sxs-lookup"><span data-stu-id="c2880-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="c2880-104">Bu çeşitli erişim kısıtlama yöntemleri aşağıda özetlenmiştir.</span><span class="sxs-lookup"><span data-stu-id="c2880-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="c2880-105">**İzin Kısıtlaması**</span><span class="sxs-lookup"><span data-stu-id="c2880-105">**Permission Restriction**</span></span>

<span data-ttu-id="c2880-106">SharePoint Online ve OneDrive for Business'ta, siteler, dosyalar ve klasörler gibi öğelere erişimi yalnızca erişimi olması gereken gruplara/kişilere erişim izni vererek kısıtlarız.</span><span class="sxs-lookup"><span data-stu-id="c2880-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="c2880-107">SharePoint listesi veya kitaplık için izinleri özelleştirme</span><span class="sxs-lookup"><span data-stu-id="c2880-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="c2880-108">SharePoint site izinlerini özelleştirme</span><span class="sxs-lookup"><span data-stu-id="c2880-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="c2880-109">Alt klasördeki izinleri değiştirme</span><span class="sxs-lookup"><span data-stu-id="c2880-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="c2880-110">Yönetilmeyen cihazlardan erişimi denetleme</span><span class="sxs-lookup"><span data-stu-id="c2880-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="c2880-111">Office 365'te SharePoint veya global yönetici olarak, yönetilmeyen aygıtlardan SharePoint ve OneDrive içeriğine erişimi engelleyebilir veya sınırlandırabilirsiniz (Karma AD'nin Intune'da katıldığı veya uyumlu olmayanlar).</span><span class="sxs-lookup"><span data-stu-id="c2880-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="c2880-112">**Ağ Konumu Kısıtlaması**</span><span class="sxs-lookup"><span data-stu-id="c2880-112">**Network Location Restriction**</span></span>

<span data-ttu-id="c2880-113">BT yöneticisi olarak, güvendiğiniz tanımlı ağ konumlarını temel alan SharePoint ve OneDrive kaynaklarına erişimi denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c2880-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="c2880-114">Bu, konum tabanlı ilke olarak da bilinir.</span><span class="sxs-lookup"><span data-stu-id="c2880-114">This is also known as location-based policy.</span></span> <span data-ttu-id="c2880-115">Daha fazla bilgi için lütfen [ağ konumuna göre SharePoint Online ve OneDrive verilerine erişimi kontrol etme](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) konusuna bakın</span><span class="sxs-lookup"><span data-stu-id="c2880-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="c2880-116">**Site Kilidi Kısıtlaması**</span><span class="sxs-lookup"><span data-stu-id="c2880-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="c2880-117">SharePoint Online'da bir site koleksiyonunu kilitleme olanağınız vardır, böylece kimsenin erişimi yoktur.</span><span class="sxs-lookup"><span data-stu-id="c2880-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="c2880-118">Bu [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState özelliği kullanılarak PowerShell ve [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) üzerinden ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="c2880-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="c2880-119">**Kullanıcıların site veya alt site oluşturmalarını kısıtlama**</span><span class="sxs-lookup"><span data-stu-id="c2880-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="c2880-120">SharePoint yöneticisi veya Office 365 global yöneticisi olarak, kullanıcılarınızın kendi SharePoint sitelerini oluşturmasına ve yönetmesine, ne tür siteler oluşturabileceklerini belirlemesine ve sitelerin konumunu belirtebildiği ne kadar sınamasına izin verebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c2880-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="c2880-121">Daha fazla bilgi için lütfen [SharePoint Online'da site oluşturmayı yönet'e](https://docs.microsoft.com/sharepoint/manage-site-creation) bakın</span><span class="sxs-lookup"><span data-stu-id="c2880-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

