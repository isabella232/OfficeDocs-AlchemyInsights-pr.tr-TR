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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719501"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a><span data-ttu-id="1940e-102">Bağlanılan site grubu SharePoint çevrimiçi oluşturun</span><span class="sxs-lookup"><span data-stu-id="1940e-102">Create group connected site in SharePoint Online</span></span>

<p><span data-ttu-id="1940e-103"><strong>Birkaç site veya bir grup oluşturarak yeniden bağlandığında karşılaşılan genel sorunlar vardır.&nbsp;</strong></span><span class="sxs-lookup"><span data-stu-id="1940e-103"><strong>There are a couple of common issues encountered when creating or re-creating a group connected site.&nbsp;</strong></span></span></p>  <p><span data-ttu-id="1940e-104">1.Bir grup ve bağlantılı sitesi silmiş ve aynı URL ile başka bir site oluşturmak istiyorsanız, önceki site kalıcı olarak kaldırmak gerekir.</span><span class="sxs-lookup"><span data-stu-id="1940e-104">1. If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span></p>  <ul>  <li><span data-ttu-id="1940e-105">Karşıdan <a title="SPO Yönetim Kabuğu</span><span class="sxs-lookup"><span data-stu-id="1940e-105">Download <a title="SPO Management Shell</span></span>" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429"><span data-ttu-id="1940e-106">SPO Yönetim Kabuğu</a> - powershell ile çalışmaya başlama hakkında daha fazla bilgi için bkz: <a title="SharePoint çevrimiçi Yönetim Kabuğu ile Başlarken</span><span class="sxs-lookup"><span data-stu-id="1940e-106">SPO Management Shell</a> - For more info on getting started with powershell, see <a title="Getting started with SharePoint Online Management Shell</span></span>" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps"><span data-ttu-id="1940e-107">SharePoint çevrimiçi Yönetim Kabuğu ile Başlarken</a>.</span><span class="sxs-lookup"><span data-stu-id="1940e-107">Getting started with SharePoint Online Management Shell</a>.</span></span> <br /><br /></li>  <li><span data-ttu-id="1940e-108">Silinen siteleri kullanarak Site kaldırma <a title="SPODeletedSite Kaldır</span><span class="sxs-lookup"><span data-stu-id="1940e-108">Remove the Site from Deleted Sites using the <a title="Remove-SPODeletedSite</span></span>" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps"><span data-ttu-id="1940e-109">Kaldır-SPODeletedSite</a> powershell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="1940e-109">Remove-SPODeletedSite</a> powershell cmdlet.</span></span></li>  </ul>  <p><span data-ttu-id="1940e-110">Bir grup bağlanılan site oluşturuyorsanız ve <strong>'zaten aynı ada sahip başka bir grup var'</strong>uyarı almak, varolan grupları denetleyin <a title="Yönetim Merkezi'nden Office 365</span><span class="sxs-lookup"><span data-stu-id="1940e-110">If you're creating a group connected site and receive a warning <strong>'Another group with the same alias already exists'</strong>, check the existing groups from the <a title="Office 365 from the Admin Center</span></span>" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups"><span data-ttu-id="1940e-111">Office 365 Yönetim Merkezi'nden</a>.</span><span class="sxs-lookup"><span data-stu-id="1940e-111">Office 365 from the Admin Center</a>.</span></span> <span data-ttu-id="1940e-112">Bu sorunu çözmek, artık gerekli değilse, varolan bir grubu silerseniz veya site ile farklı bir diğer ad oluşturmak için atanmış.&nbsp;</span><span class="sxs-lookup"><span data-stu-id="1940e-112">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.&nbsp;</span></span></p>  <p><span data-ttu-id="1940e-113"><strong>Oluşturmak ve SharePoint ile modern grupları kullanmak için farklı yolları vardır.&nbsp;</strong></span><span class="sxs-lookup"><span data-stu-id="1940e-113"><strong>There are different ways to create and use modern groups with SharePoint.&nbsp;</strong></span></span></p>  <ol>  <li><span data-ttu-id="1940e-114">Bir Office 365 gruba varolan sitelere bağlanabilir.</span><span class="sxs-lookup"><span data-stu-id="1940e-114">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="1940e-115">Daha fazla bilgi için bkz: <a title="SharePoint kullanıcı ineterface kullanarak bir Office 365 Grup bağlanma</span><span class="sxs-lookup"><span data-stu-id="1940e-115">For more info, see <a title="Connect an Office 365 group using the SharePoint user ineterface</span></span>" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface"><span data-ttu-id="1940e-116">SharePoint kullanıcı ineterface kullanarak bir Office 365 Grup bağlanmak</a>.</span><span class="sxs-lookup"><span data-stu-id="1940e-116">Connect an Office 365 group using the SharePoint user ineterface</a>.</span></span></li>  <li><span data-ttu-id="1940e-117">Office 365 Grup bağlanılan site oluşturmak için bir ekip sitesi oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="1940e-117">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="1940e-118">Daha fazla bilgi için bkz: <a title="içinde SharePoint ekip sitesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="1940e-118">For more info, see <a title="Create a team site in SharePoint</span></span>" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d"><span data-ttu-id="1940e-119">SharePoint'te ekip sitesi oluşturun.</a></span><span class="sxs-lookup"><span data-stu-id="1940e-119">Create a team site in SharePoint.</a></span></span></li>  </ol>
