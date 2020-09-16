---
title: SharePoint sitesine grup ekleme
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771228"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="0647b-102">SharePoint 'te grup bağlantılı sitesi oluştururken karşılaşılan sorunlar</span><span class="sxs-lookup"><span data-stu-id="0647b-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="0647b-103">Grup bağlantılı bir siteyi oluştururken veya yeniden oluştururken karşılaşılan bazı yaygın sorunlar oluştu.</span><span class="sxs-lookup"><span data-stu-id="0647b-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="0647b-104">Bir grubu ve bağlı siteyi sildiyseniz ve aynı URL 'ye sahip başka bir site oluşturmak istiyorsanız, önceki siteyi kalıcı olarak kaldırmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="0647b-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="0647b-105">[SPO Yönetim Kabuğu 'nu](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) indirin</span><span class="sxs-lookup"><span data-stu-id="0647b-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="0647b-106">PowerShell ile çalışmaya başlama hakkında daha fazla bilgi için [SharePoint Online Yönetim Kabuğu ile çalışmaya](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)başlama konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="0647b-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="0647b-107">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell cmdlet 'Ini kullanarak siteyi silinmiş sitelerden kaldırın.</span><span class="sxs-lookup"><span data-stu-id="0647b-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="0647b-108">Grup sitelerini kalıcı olarak silmek için PowerShell gereklidir.</span><span class="sxs-lookup"><span data-stu-id="0647b-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="0647b-109">Grup bağlantılı bir site oluşturuyorsanız ve bir uyarı alırsanız: **aynı diğer ada sahip başka bir grup zaten varsa**, [Microsoft 365 Yönetim merkezinden](https://admin.microsoft.com/AdminPortal/Home#/groups)var olan grupları işaretleyin.</span><span class="sxs-lookup"><span data-stu-id="0647b-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="0647b-110">Sorunu çözmek için, artık gerekmiyorsa var olan grubu silin veya başka bir diğer adla atanmış olan siteyi silin.</span><span class="sxs-lookup"><span data-stu-id="0647b-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="0647b-111">SharePoint ile modern gruplar oluşturmanın ve kullanmanın farklı yolları vardır.</span><span class="sxs-lookup"><span data-stu-id="0647b-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="0647b-112">Var olan siteleri Microsoft 365 grubuna bağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0647b-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="0647b-113">Daha fazla bilgi için [SharePoint kullanıcı arabirimini kullanarak Microsoft 365 grubunu bağlama](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="0647b-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="0647b-114">Microsoft 365 Group bağlantılı sitesi oluşturmak için [ekip sitesi](https://admin.microsoft.com/sharepoint)oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="0647b-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
