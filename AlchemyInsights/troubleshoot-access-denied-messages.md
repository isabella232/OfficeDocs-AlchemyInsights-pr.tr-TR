---
title: Erişim reddedildi iletilerinde sorun giderme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690803"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="d7e20-102">Erişim reddedildi iletilerinde sorun giderme</span><span class="sxs-lookup"><span data-stu-id="d7e20-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="d7e20-103">SharePoint 'te paylaşılan bir klasöre "erişim reddedildi" iletisi varsa, site koleksiyonu Yöneticisi "sınırlı erişimli kullanıcı izni kilitleme modu" seçeneğini etkinleştirmiş olabilir.</span><span class="sxs-lookup"><span data-stu-id="d7e20-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="d7e20-104">Bunu kapatmak için:</span><span class="sxs-lookup"><span data-stu-id="d7e20-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="d7e20-105">Siteye gidin, ayarlar simgesini ve sonra **site ayarları**'nı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d7e20-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="d7e20-106">**Site koleksiyonu yönetimi**'nin altında, **site koleksiyonu özellikleri**'ni tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d7e20-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="d7e20-107">**Sınırlı erişimli kullanıcı izni kilitleme modu**'Nun yanında **devre dışı bırak**'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d7e20-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="d7e20-108">Site bir yayımlama sitesidir, paylaşılan klasörler için de erişim reddedildi iletisi görüntülenebilir.</span><span class="sxs-lookup"><span data-stu-id="d7e20-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="d7e20-109">Bilgi için, [paylaşılan klasöre erişirken erişim reddedildi](https://go.microsoft.com/fwlink/?linkid=2004317)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="d7e20-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="d7e20-110">Erişim isteklerini görüntülemeye çalışırken bir "erişim reddedildi" iletisi varsa, kullanıcının site koleksiyonu Yöneticisi veya site için sahipler grubunun üyesi olarak eklenmesi gereklidir.</span><span class="sxs-lookup"><span data-stu-id="d7e20-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="d7e20-111">Daha fazla bilgi için bkz [.](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="d7e20-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="d7e20-112">Bir kullanıcı şirket içi Active Directory 'den kaldırıldıktan sonra "erişim reddedildi" iletisiyle karşılaştıklarında, bir [Kullanıcı hesabı Microsoft 365 ile eşitlendiğinde erişim reddedildi](https://go.microsoft.com/fwlink/?linkid=2004318)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="d7e20-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

