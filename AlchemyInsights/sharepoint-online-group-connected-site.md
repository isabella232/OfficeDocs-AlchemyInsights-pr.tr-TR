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
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051121"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="103c4-102">SharePoint Online'da bağlı siteler oluştururken veya gruplandırmada sorunlar</span><span class="sxs-lookup"><span data-stu-id="103c4-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="103c4-103">Grup bağlantılı bir site oluştururken veya yeniden oluştururken karşılaşılan birkaç yaygın sorun vardır.</span><span class="sxs-lookup"><span data-stu-id="103c4-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="103c4-104">Bir grubu ve bağlı sitesini sildiyseniz ve aynı URL'ye sahip başka bir site oluşturmak istiyorsanız, önceki siteyi kalıcı olarak kaldırmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="103c4-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="103c4-105">Karşıdan yükleme [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="103c4-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="103c4-106">Powershell ile başlamak hakkında daha fazla bilgi için [SharePoint Online Management Shell ile başlarken](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="103c4-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="103c4-107">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet kullanarak Siteyi Silinmiş Sitelerden kaldırın.</span><span class="sxs-lookup"><span data-stu-id="103c4-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="103c4-108">Grup bağlantılı bir site oluşturuyorsanız ve bir uyarı alıyorsanız, aynı takma ada sahip başka bir grup zaten var, [Yönetici Merkezi'nden Office 365'teki](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)varolan grupları denetleyin.</span><span class="sxs-lookup"><span data-stu-id="103c4-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="103c4-109">Sorunu gidermek için, artık gerekli değilse varolan grubu silin veya farklı bir takma ad atanmış siteyi oluşturun.</span><span class="sxs-lookup"><span data-stu-id="103c4-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="103c4-110">SharePoint ile modern gruplar oluşturmanın ve kullanmanın farklı yolları vardır.</span><span class="sxs-lookup"><span data-stu-id="103c4-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="103c4-111">Varolan siteleri bir Office 365 grubuna bağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="103c4-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="103c4-112">Daha fazla bilgi için [bkz.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)</span><span class="sxs-lookup"><span data-stu-id="103c4-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="103c4-113">Office 365 grubuna bağlı bir site oluşturmak için bir Ekip Sitesi oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="103c4-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="103c4-114">Daha fazla bilgi için bkz: [SharePoint'te bir ekip sitesi oluştur.](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)</span><span class="sxs-lookup"><span data-stu-id="103c4-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

