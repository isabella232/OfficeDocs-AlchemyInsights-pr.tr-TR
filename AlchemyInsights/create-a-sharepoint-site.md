---
title: Bir SharePoint sitesi oluşturma
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ad1a77b69d2d453dbd3daa304759238b329f96ba
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269936"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="c45c5-102">Bir SharePoint sitesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="c45c5-102">Create a SharePoint site</span></span>

<span data-ttu-id="c45c5-103">SharePoint sitesi oluşturma hakkında bilgi için aşağıdakileri görebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="c45c5-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="c45c5-104">[Yeni SharePoint Yönetim Merkezi'ndeki siteleri yönetme](https://docs.microsoft.com/sharepoint/manage-site-creation): Klasik bir site veya Office 365 Grup içermez bir ekip sitesi oluşturma dahil olmak üzere site oluşturma seçenekleri hakkında bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="c45c5-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="c45c5-105">[SharePoint ekip sitesinde oluşturma](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): bir ekip sitesi oluşturmayı öğrenin.</span><span class="sxs-lookup"><span data-stu-id="c45c5-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="c45c5-106">[SharePoint çevrimiçi iletişim sitesi oluştur](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): iletişim site oluşturmayı öğrenin.</span><span class="sxs-lookup"><span data-stu-id="c45c5-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="c45c5-107">[Yeni SharePoint Yönetim Merkezi'ndeki siteleri yönetme](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Klasik bir site veya bir Office 365 Grup içermediği bir ekip sitesi oluşturmayı öğrenin.</span><span class="sxs-lookup"><span data-stu-id="c45c5-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! İpuçları]
> - <span data-ttu-id="c45c5-109">Varolan bir sitenin aynı URL'ye bir site oluşturamazsınız.</span><span class="sxs-lookup"><span data-stu-id="c45c5-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="c45c5-110">Site silindiğinde ve yeniden URL kullanmak isteyen, silinmiş bir site altında **Silinmiş siteler**hala varolduğunu mümkündür.</span><span class="sxs-lookup"><span data-stu-id="c45c5-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="c45c5-111">Yönetmek için siteleri bkz:, [siteyi silebileceği](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)sildi.</span><span class="sxs-lookup"><span data-stu-id="c45c5-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="c45c5-112">Bir site Powershell ile tümüyle kaldırmak için [Kaldır-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet örneğe bakın.</span><span class="sxs-lookup"><span data-stu-id="c45c5-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="c45c5-113">Bazı kullanıcılar site oluşturmak mümkün olmayabilir.</span><span class="sxs-lookup"><span data-stu-id="c45c5-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="c45c5-114">[Yönet Online'da SharePoint sitesi oluşturma](https://docs.microsoft.com/sharepoint/manage-site-creation)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="c45c5-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="c45c5-115">Site **oluşturma** sırasında beklenenden uzun takılmış görünüyor mümkündür.</span><span class="sxs-lookup"><span data-stu-id="c45c5-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="c45c5-116">Bu sorun ilk gördüğünüz bu yana 24 saatten fazla başarılı olması halinde, Lütfen bir destek bileti oturum.</span><span class="sxs-lookup"><span data-stu-id="c45c5-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="c45c5-117">Çoğu durumda, biz zaten bir çözüm üzerinde çalışıyorsunuz.</span><span class="sxs-lookup"><span data-stu-id="c45c5-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="c45c5-118">Lütfen bize bir çözüm tamamlamak için en az 24 saat verin.</span><span class="sxs-lookup"><span data-stu-id="c45c5-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="c45c5-119">Office 365 grup içeren yeni bir ekip sitesi oluşturmanız gerekiyorsa,</span><span class="sxs-lookup"><span data-stu-id="c45c5-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


