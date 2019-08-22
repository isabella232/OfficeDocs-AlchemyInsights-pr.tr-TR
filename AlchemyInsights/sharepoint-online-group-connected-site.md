---
title: Bir grup için bir SharePoint sitesi ekleme
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507867"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="710be-102">Çevrimiçi SharePoint siteleri oluşturma veya gruba bağlı sorunlar</span><span class="sxs-lookup"><span data-stu-id="710be-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="710be-103">Birkaç site veya bir grup oluşturarak yeniden bağlandığında karşılaşılan genel sorunlar vardır.</span><span class="sxs-lookup"><span data-stu-id="710be-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="710be-104">Bir grup ve bağlantılı sitesi silmiş ve aynı URL ile başka bir site oluşturmak istiyorsanız, önceki site kalıcı olarak kaldırmak gerekir.</span><span class="sxs-lookup"><span data-stu-id="710be-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="710be-105">[SPO Yönetim Kabuğu'nu](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) indirin</span><span class="sxs-lookup"><span data-stu-id="710be-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="710be-106">Powershell ile çalışmaya başlama hakkında daha fazla bilgi için bkz: [SharePoint çevrimiçi Yönetim Kabuğu ile Başlarken](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="710be-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="710be-107">Siteyi [Kaldır-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet'ini kullanarak siteleri silinmiş kaldırmak.</span><span class="sxs-lookup"><span data-stu-id="710be-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="710be-108">Bir grup bağlanılan site oluşturuyorsanız ve aynı ada sahip başka bir grup zaten var olan bir uyarı alırsınız, varolan [Office 365 Yönetim Merkezi'nden](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)gruplarından denetleyin.</span><span class="sxs-lookup"><span data-stu-id="710be-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="710be-109">Bu sorunu çözmek, artık gerekli değilse, varolan bir grubu silerseniz veya site ile farklı bir diğer ad oluşturmak için atanmış.</span><span class="sxs-lookup"><span data-stu-id="710be-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="710be-110">Oluşturmak ve SharePoint ile modern grupları kullanmak için farklı yolları vardır.</span><span class="sxs-lookup"><span data-stu-id="710be-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="710be-111">Bir Office 365 gruba varolan sitelere bağlanabilir.</span><span class="sxs-lookup"><span data-stu-id="710be-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="710be-112">Daha fazla bilgi için bkz: [SharePoint kullanıcı ineterface kullanarak bir Office 365 Grup Bağlan](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="710be-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="710be-113">Office 365 Grup bağlanılan site oluşturmak için bir ekip sitesi oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="710be-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="710be-114">Daha fazla bilgi için bkz: [SharePoint ekip sitesinde oluşturma](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="710be-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

