---
title: Erişim Reddedilen iletileri sorun giderme
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050725"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="d4ab4-102">Erişim Reddedilen iletileri sorun giderme</span><span class="sxs-lookup"><span data-stu-id="d4ab4-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="d4ab4-103">Birisi SharePoint'te paylaşılan bir klasöre "Erişim Reddedildi" iletisi aldıysa, site koleksiyonu yöneticisi "Sınırlı erişimli kullanıcı izni kilitleme modunu" etkinleştirmiş olabilir.</span><span class="sxs-lookup"><span data-stu-id="d4ab4-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="d4ab4-104">Bunu kapatmak için:</span><span class="sxs-lookup"><span data-stu-id="d4ab4-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="d4ab4-105">Siteye göz atın, Ayarlar simgesine tıklayın ve ardından **Site Ayarları'nı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d4ab4-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="d4ab4-106">**Site Toplama İdaresi**altında, Site koleksiyonu **özelliklerini**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d4ab4-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="d4ab4-107">Sınırlı **erişimli kullanıcı izni kilitleme modunun**yanında **Devre Dışı bırak'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d4ab4-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="d4ab4-108">Site bir yayımlama sitesiyse, paylaşılan klasörler için erişim engellendi iletisi de oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="d4ab4-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="d4ab4-109">Daha fazla bilgi için, [paylaşılan bir klasöre erişirken Erişim Reddedildi'ye](https://go.microsoft.com/fwlink/?linkid=2004317)bakın.</span><span class="sxs-lookup"><span data-stu-id="d4ab4-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="d4ab4-110">Bir kişi erişim isteklerini görüntülemeye çalışırken "Erişim Reddedildi" iletisi aldıysa, kullanıcının site koleksiyonu yöneticisi veya sitenin Sahipleri grubunun bir üyesi olarak eklenmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="d4ab4-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="d4ab4-111">Daha fazla bilgi için erişim [isteklerine erişim engellendi listesine](https://go.microsoft.com/fwlink/?linkid=2004220)bakın.</span><span class="sxs-lookup"><span data-stu-id="d4ab4-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="d4ab4-112">Bir kullanıcı, Şirket içinde Active Directory'den kaldırıldıktan ve sonra geri eklendikten sonra bir "Erişim Reddedildi" iletisi aldıysa, [kullanıcı hesabı Office 365 ile senkronize edildiğinde Erişim Reddedildi'ye](https://go.microsoft.com/fwlink/?linkid=2004318)bakın.</span><span class="sxs-lookup"><span data-stu-id="d4ab4-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

