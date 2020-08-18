---
title: SharePoint sitesi oluşturma
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: ba682f3c2b2600031f6856621691b1e0fba64113
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786585"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="7b2d8-102">SharePoint sitesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="7b2d8-102">Create a SharePoint site</span></span>

<span data-ttu-id="7b2d8-103">SharePoint Yönetim merkezinde [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) 'de site oluşturma veya yönetme.</span><span class="sxs-lookup"><span data-stu-id="7b2d8-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="7b2d8-104">Daha fazla bilgi için [Yeni SharePoint Yönetim merkezinde siteleri yönetme](https://docs.microsoft.com/sharepoint/manage-site-creation)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="7b2d8-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="7b2d8-105">Ok</span><span class="sxs-lookup"><span data-stu-id="7b2d8-105">Tips:</span></span>

- <span data-ttu-id="7b2d8-106">Var olan bir sitenin URL 'sini içeren bir **site oluşturamazsınız.**</span><span class="sxs-lookup"><span data-stu-id="7b2d8-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="7b2d8-107">Bir siteyi sildiyseniz ve URL 'YI yeniden kullanmayı düşünüyorsanız, silinen site yine [Silinmiş sitelerde](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)yer alabilir.</span><span class="sxs-lookup"><span data-stu-id="7b2d8-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="7b2d8-108">URL 'YI yeniden kullanmak için sitenin kalıcı olarak silinmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="7b2d8-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="7b2d8-109">Bir siteyi PowerShell ile tümüyle kaldırmak için [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet 'ine bakın.</span><span class="sxs-lookup"><span data-stu-id="7b2d8-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="7b2d8-110">Bazı kullanıcılar site oluşturamaz.</span><span class="sxs-lookup"><span data-stu-id="7b2d8-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="7b2d8-111">[SharePoint Online 'da site oluşturmayı yönetme konusuna bakın](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="7b2d8-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="7b2d8-112">Site **beklenenden uzun süre** içinde kalmış görünüyor.</span><span class="sxs-lookup"><span data-stu-id="7b2d8-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="7b2d8-113">Bu sorunu ilk kez gördüğünüzde 24 saatten uzun bir süreyi geçmişse, lütfen bir destek bileti günlüğe yazılır.</span><span class="sxs-lookup"><span data-stu-id="7b2d8-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="7b2d8-114">Birçok durumda bir çözüm üzerinde çalışıyoruz.</span><span class="sxs-lookup"><span data-stu-id="7b2d8-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="7b2d8-115">Lütfen çözümü tamamlamak için en az 24 saat bekleyin.</span><span class="sxs-lookup"><span data-stu-id="7b2d8-115">Please give us at least 24 hours to complete a solution.</span></span>
