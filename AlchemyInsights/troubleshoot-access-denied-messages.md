---
title: Erişim Reddedildi ileti sorunlarını giderme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704914"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="91388-102">Erişim Reddedildi ileti sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="91388-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="91388-103">Birisi SharePoint'te paylaşılan bir klasöre "Erişim Reddedildi" iletisi aldısa, site koleksiyonu yöneticisi "Sınırlı erişimli kullanıcı izni kilitleme modu" etkinleştirmiş olabilir.</span><span class="sxs-lookup"><span data-stu-id="91388-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="91388-104">Bunu kapatmak için:</span><span class="sxs-lookup"><span data-stu-id="91388-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="91388-105">Siteye gidin, Ayarlar simgesine tıklayın ve sonra da **Site Ayarları'ne tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="91388-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="91388-106">Site **Koleksiyonu Yönetimi'nin altında** Site koleksiyonu **özellikleri'ne tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="91388-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="91388-107">Sınırlı **erişimli kullanıcı izni kilitleme modunun yanında Devre Dışı Bırak'a** **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="91388-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="91388-108">Site bir yayımlama sitesi olduğunda, paylaşılan klasörler için Erişim Reddedildi iletisi de oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="91388-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="91388-109">Bilgi için bkz. [Paylaşılan klasöre erişirken Erişim Reddedildi.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)</span><span class="sxs-lookup"><span data-stu-id="91388-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="91388-110">Erişim isteklerini görüntülemeye çalışırken bir kullanıcı "Erişim Reddedildi" iletisi alıyorsa, kullanıcının site için site koleksiyonu yöneticisi veya Sahipler grubunun bir üyesi olarak ekleniyor olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="91388-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="91388-111">Daha fazla bilgi için erişim [reddedildi erişim istekleri listesine bakın.](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="91388-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="91388-112">Kullanıcı Active Directory'den şirket içinde kaldırıldıktan sonra "Erişim Reddedildi" iletisi aldı ve sonra yeniden eklendikten sonra kullanıcı hesabı [Microsoft 365'e](https://go.microsoft.com/fwlink/?linkid=2004318)eşitleniyorsa Erişim Reddedildi iletisine bakın.</span><span class="sxs-lookup"><span data-stu-id="91388-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

