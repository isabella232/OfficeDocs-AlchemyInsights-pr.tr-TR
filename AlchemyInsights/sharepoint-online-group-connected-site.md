---
title: SharePoint sitesine grup ekleme
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8ef33cbd44b01deaf0e45813d019f7696ef5def0
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912986"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="639a9-102">SharePoint'te grup bağlantılı bir site oluştururken sorunlar</span><span class="sxs-lookup"><span data-stu-id="639a9-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="639a9-103">Grup bağlantılı bir site oluştururken veya yeniden oluştururken karşılaşılan bazı yaygın sorunlar.</span><span class="sxs-lookup"><span data-stu-id="639a9-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="639a9-104">Bir grubu ve bağlı sitesini sildiyseniz ve aynı URL'ye sahip başka bir site oluşturmak istiyorsanız, önceki siteyi kalıcı olarak kaldırmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="639a9-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="639a9-105">Karşıdan yükleme [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="639a9-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="639a9-106">Powershell ile başlamak hakkında daha fazla bilgi için [SharePoint Online Management Shell ile başlarken](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)bakın.</span><span class="sxs-lookup"><span data-stu-id="639a9-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="639a9-107">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet kullanarak Siteyi Silinmiş Sitelerden kaldırın.</span><span class="sxs-lookup"><span data-stu-id="639a9-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="639a9-108">Powershell'in grup sitelerini kalıcı olarak silmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="639a9-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="639a9-109">Grup bağlantılı bir site oluşturuyorsanız ve bir uyarı alıyorsanız: **Aynı takma ada sahip başka bir grup zaten var,** [Microsoft 365 Yönetici Merkezi'nden](https://admin.microsoft.com/AdminPortal/Home#/groups)varolan grupları denetleyin.</span><span class="sxs-lookup"><span data-stu-id="639a9-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="639a9-110">Sorunu gidermek için, artık gerekli değilse varolan grubu silin veya farklı bir takma ad atanmış siteyi oluşturun.</span><span class="sxs-lookup"><span data-stu-id="639a9-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="639a9-111">SharePoint ile modern gruplar oluşturmanın ve kullanmanın farklı yolları vardır.</span><span class="sxs-lookup"><span data-stu-id="639a9-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="639a9-112">Varolan siteleri bir Microsoft 365 grubuna bağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="639a9-112">You can connect existing sites to an Microsoft 365 group.</span></span> <span data-ttu-id="639a9-113">Daha fazla bilgi için bkz: [SharePoint kullanıcı arabirimini kullanarak bir Microsoft 365 grubunu bağlayın.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)</span><span class="sxs-lookup"><span data-stu-id="639a9-113">For more info, see [Connect an Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="639a9-114">Microsoft 365 grubuna bağlı bir site oluşturmak için bir [Ekip Sitesi](https://admin.microsoft.com/sharepoint)oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="639a9-114">To create an Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
