---
title: SharePoint veya OneDrive 'da erişimi kısıtlama
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700475"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="a0920-102">SharePoint veya OneDrive 'da erişimi kısıtlama</span><span class="sxs-lookup"><span data-stu-id="a0920-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="a0920-103">SharePoint Online/OneDrive hizmetlerine erişimi sınırlandırmanın birçok yolu vardır.</span><span class="sxs-lookup"><span data-stu-id="a0920-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="a0920-104">Bu çeşitli erişim kısıtlama yöntemleri aşağıda özetlenmiştir.</span><span class="sxs-lookup"><span data-stu-id="a0920-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="a0920-105">**İzin kısıtlaması**</span><span class="sxs-lookup"><span data-stu-id="a0920-105">**Permission Restriction**</span></span>

<span data-ttu-id="a0920-106">SharePoint Online ve OneDrive Iş 'te, yalnızca erişmesi gereken gruplara/kişilere erişim vererek site, dosya ve klasör gibi öğelere erişimi kısıtlıyoruz.</span><span class="sxs-lookup"><span data-stu-id="a0920-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="a0920-107">SharePoint listesi veya kitaplığı için izinleri özelleştirme</span><span class="sxs-lookup"><span data-stu-id="a0920-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="a0920-108">SharePoint sitesi izinlerini özelleştirme</span><span class="sxs-lookup"><span data-stu-id="a0920-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="a0920-109">Alt klasördeki izinleri değiştirme</span><span class="sxs-lookup"><span data-stu-id="a0920-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="a0920-110">Yönetilmeyen cihazlardan erişimi denetleme</span><span class="sxs-lookup"><span data-stu-id="a0920-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="a0920-111">SharePoint veya genel yönetici olarak, yönetilmeyen cihazlardan SharePoint ve OneDrive içeriğine erişimi engelleyebilir veya sınırlayabilir (karma AD 'a bağlı olmayan veya Intune 'da uyumlu olanlar).</span><span class="sxs-lookup"><span data-stu-id="a0920-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="a0920-112">**Ağ konumu kısıtlaması**</span><span class="sxs-lookup"><span data-stu-id="a0920-112">**Network Location Restriction**</span></span>

<span data-ttu-id="a0920-113">BT Yöneticisi olarak, güvendiğiniz ağ konumlarına göre SharePoint ve OneDrive kaynaklarına erişimi denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a0920-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="a0920-114">Bu, konum tabanlı ilke olarak da bilinir.</span><span class="sxs-lookup"><span data-stu-id="a0920-114">This is also known as location-based policy.</span></span> <span data-ttu-id="a0920-115">Daha fazla bilgi için bkz: [SharePoint Online ve OneDrive verilerine ağ konumuna göre denetleme](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="a0920-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="a0920-116">**Site kilit sınırlaması**</span><span class="sxs-lookup"><span data-stu-id="a0920-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="a0920-117">SharePoint Online 'da site koleksiyonunu kilitleme olanağınız vardır, dolayısıyla kimse erişimi yoktur.</span><span class="sxs-lookup"><span data-stu-id="a0920-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="a0920-118">Bu, [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate özelliği kullanılarak PowerShell ve [SharePoint Online Yönetim Kabuğu](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ile ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="a0920-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="a0920-119">**Kullanıcıların site veya alt site oluşturmasını kısıtlama**</span><span class="sxs-lookup"><span data-stu-id="a0920-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="a0920-120">SharePoint Yöneticisi veya genel yönetici olarak, kullanıcılarınızın kendi SharePoint sitelerini oluşturmasına ve yönetmesine, oluşturabildikleri site türlerini belirlemesine ve sitelerin konumunu belirlemesine izin verebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a0920-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="a0920-121">Daha fazla bilgi için bkz: [SharePoint Online 'da site oluşturmayı yönetme](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="a0920-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

