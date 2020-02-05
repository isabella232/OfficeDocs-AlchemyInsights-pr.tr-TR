---
title: SharePoint sitesi oluşturma
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770875"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="5d968-102">SharePoint sitesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="5d968-102">Create a SharePoint site</span></span>

<span data-ttu-id="5d968-103">SharePoint Yönetici Merkezi'ndeki [Etkin Siteler'den](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) siteler oluşturun veya yönetin.</span><span class="sxs-lookup"><span data-stu-id="5d968-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="5d968-104">Daha fazla bilgi için, [yeni SharePoint yönetici merkezindeki siteleri yönet'e](https://docs.microsoft.com/sharepoint/manage-site-creation)bakın.</span><span class="sxs-lookup"><span data-stu-id="5d968-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="5d968-105">Ipuç -ları:</span><span class="sxs-lookup"><span data-stu-id="5d968-105">Tips:</span></span>

- <span data-ttu-id="5d968-106">Varolan bir sitenin aynı URL'sini içeren bir site **oluşturamazsınız.**</span><span class="sxs-lookup"><span data-stu-id="5d968-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="5d968-107">Bir siteyi sildiyseniz ve URL'yi yeniden kullanmak istiyorsanız, silinen site [silinmiş sitelerin](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)altında hala var olabilir.</span><span class="sxs-lookup"><span data-stu-id="5d968-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="5d968-108">URL'yi yeniden kullanmak için sitenin kalıcı olarak silinmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="5d968-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="5d968-109">Powershell içeren bir siteyi tamamen kaldırmak [için, Kaldır-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet örneğine bakın.</span><span class="sxs-lookup"><span data-stu-id="5d968-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="5d968-110">Bazı kullanıcılar bir site oluşturamayabilir.</span><span class="sxs-lookup"><span data-stu-id="5d968-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="5d968-111">[Bkz. SharePoint Online'da site oluşturmayı yönet.](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="5d968-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="5d968-112">Sitenin beklenenden daha uzun süredir **Oluşturma'da** sıkışmış görünmesi mümkündür.</span><span class="sxs-lookup"><span data-stu-id="5d968-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="5d968-113">Bu sorunu ilk gördüğünüzden bu yana 24 saatten fazla zaman geçtiyse, lütfen bir destek bileti ni kaydedin.</span><span class="sxs-lookup"><span data-stu-id="5d968-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="5d968-114">Çoğu durumda, zaten bir çözüm üzerinde çalışıyoruz.</span><span class="sxs-lookup"><span data-stu-id="5d968-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="5d968-115">Lütfen bir çözümü tamamlamamız için bize en az 24 saat verin.</span><span class="sxs-lookup"><span data-stu-id="5d968-115">Please give us at least 24 hours to complete a solution.</span></span>
