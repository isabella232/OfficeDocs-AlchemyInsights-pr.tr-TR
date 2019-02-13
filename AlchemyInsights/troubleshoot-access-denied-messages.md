---
title: Erişim reddedildi iletisi ile ilgili sorunları giderme
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f1a4803838b6511ef4fe7f03cafa4aa13b3c9734
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916472"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="6f9f2-102">Erişim reddedildi iletisi ile ilgili sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="6f9f2-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="6f9f2-p101">Birisi bir "Erişim reddedildi" iletisi bir paylaşılan klasöre geldiyseniz, site koleksiyonu yöneticisi "sınırlı erişimli kullanıcı izni kilitleme modu" etkin Bunu kapatmak için:</span><span class="sxs-lookup"><span data-stu-id="6f9f2-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="6f9f2-105">Siteye göz atın, Ayarlar simgesini tıklatın ve ardından **Site Ayarları**' nı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="6f9f2-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="6f9f2-106">**Site Koleksiyonu Yönetimi**altında **Site koleksiyonu özellikleri**' ni tıklatın.</span><span class="sxs-lookup"><span data-stu-id="6f9f2-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="6f9f2-107">**Sınırlı erişimli kullanıcı izni kilitleme modu**yanındaki **devre dışı bırak**' ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="6f9f2-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="6f9f2-p102">Bir yayımlama sitesinin site ise, paylaşılan klasörler için erişim reddedildi iletisi da ortaya çıkabilir. Bilgi için bkz: [Paylaşılan klasöre erişirken erişim engellendi](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="6f9f2-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="6f9f2-p103">Birisi bir erişim isteklerini görüntülemeye çalışırken bir "Erişim engellendi" iletisi alındı, kullanıcının site koleksiyonu yöneticisi veya site sahipleri grubunun üyesi olarak eklenmesi gerekir. Daha fazla bilgi için bkz: [Erişim isteklerini listesine erişim engellendi](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="6f9f2-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="6f9f2-112">Yerinde Active Directory kaldırıldı ve başa eklenen sonra kullanıcı bir "Erişim engellendi" iletisi alındı, [Bir kullanıcı hesabı için Office 365 eşitlendiğinde, erişim engellendi](https://go.microsoft.com/fwlink/?linkid=2004318)bakın.</span><span class="sxs-lookup"><span data-stu-id="6f9f2-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

