---
title: Modern site kök site olarak
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057791"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="65df0-102">Modern site kök site olarak</span><span class="sxs-lookup"><span data-stu-id="65df0-102">Modern site as root site</span></span>

<span data-ttu-id="65df0-103">[Hedef sürüm](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) müşteriler artık Klasik kök sitesinde kendi SharePoint Kiracı, modern iletişim site deneyimini etkinleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="65df0-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="65df0-104">Bu özellik, basit bir PowerShell cmdlet'ini çalıştırarak etkinleştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="65df0-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="65df0-105">PowerShell command(s) başarılı yürütülmesine kök sitesi iletişim site giriş sayfası olacaktır.</span><span class="sxs-lookup"><span data-stu-id="65df0-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="65df0-106">PowerShell cmdlet ve özellik gereksinimleri hakkındaki ayrıntıları [Etkinleştir SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps)makalesinde bulunmaktadır.</span><span class="sxs-lookup"><span data-stu-id="65df0-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="65df0-107">Biz yavaş yavaş bu çıkışı, kapalı erken Mayıs 2019 yayın hedeflenen müşterilere varsayılan olarak çalışırken ve Top dışarı tüm dünyada Haziran 2019 sonuna kadar kullanılabilir olacaktır.</span><span class="sxs-lookup"><span data-stu-id="65df0-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="65df0-108">[İleti Merkezi](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) için diğer yeni özellikleri ile Modern başvurmak devam edin.</span><span class="sxs-lookup"><span data-stu-id="65df0-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="65df0-109">**Önemli**: modern iletişim Site oluşturmak için Klasik kök site silmeyin.</span><span class="sxs-lookup"><span data-stu-id="65df0-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="65df0-110">Bu Microsoft tarafından desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="65df0-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="65df0-111">Siteyi geri yüklemek veya aynı URL'de yeni bir site oluşturmak kadar kök site silindiğinde tüm SharePoint siteleri, kuruluşunuzdaki tüm kullanıcılar için erişilebilir hale getirir.</span><span class="sxs-lookup"><span data-stu-id="65df0-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 