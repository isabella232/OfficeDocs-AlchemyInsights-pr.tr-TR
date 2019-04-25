---
title: Bir SharePoint sitesi oluşturma
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: a4c6029c632178136396a91ba9754752dc8f7180
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32407634"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="d56e5-102">Bir SharePoint sitesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="d56e5-102">Create a SharePoint site</span></span>

<span data-ttu-id="d56e5-103">[Siteleri yönetme yeni SharePoint Yönetim Merkezi'ndeki](https://docs.microsoft.com/sharepoint/manage-site-creation ) site oluşturma seçenekleri için bkz.</span><span class="sxs-lookup"><span data-stu-id="d56e5-103">See [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation ) for site creation options.</span></span> <span data-ttu-id="d56e5-104">(Hangi Office 365 grubu oluşturur) bir [ekip sitesi](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US) veya bir [iletişim sitesi](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)oluşturmak için bu seçeneği seçin.</span><span class="sxs-lookup"><span data-stu-id="d56e5-104">Select to create a [team site](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US) (which will create an Office 365 group) or a [communication site](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb).</span></span> <span data-ttu-id="d56e5-105">[Klasik site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site)veya Office 365 grup içeren yeni bir ekip sitesi oluşturmak için **diğer seçenekler**' i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d56e5-105">To create a [classic site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site), or a new team site that doesn't include an Office 365 group, click **Other options**.</span></span> 
  
<span data-ttu-id="d56e5-106">İpuçları:</span><span class="sxs-lookup"><span data-stu-id="d56e5-106">Tips:</span></span>
- <span data-ttu-id="d56e5-107">*Varolan bir sitenin aynı URL'ye bir site oluşturamazsınız. Site silindiğinde ve yeniden URL kullanmak isteyen, silinmiş bir site altında **Silinmiş siteler**hala varolduğunu mümkündür. Yönetmek için siteleri bkz:, [siteyi silebileceği](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)sildi. Bir site Powershell ile tümüyle kaldırmak için [Kaldır-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet örneğe bakın.*</span><span class="sxs-lookup"><span data-stu-id="d56e5-107">*You cannot create a site with the same URL of an existing site. If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**. To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site). To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.*</span></span>
- <span data-ttu-id="d56e5-108">*Bazı kullanıcılar site oluşturmak mümkün olmayabilir. [Yönet Online'da SharePoint sitesi oluşturma](https://docs.microsoft.com/sharepoint/manage-site-creation)konusuna bakın.*</span><span class="sxs-lookup"><span data-stu-id="d56e5-108">*Some users may not be able to create a site. See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).*</span></span>
- <span data-ttu-id="d56e5-109">*Site **oluşturma** sırasında beklenenden uzun takılmış görünüyor mümkündür. Bu sorun ilk gördüğünüz bu yana 24 saatten fazla başarılı olması halinde, Lütfen bir destek bileti oturum. Çoğu durumda, biz zaten bir çözüm üzerinde çalışıyorsunuz. Lütfen bize bir çözüm tamamlamak için en az 24 saat verin.*</span><span class="sxs-lookup"><span data-stu-id="d56e5-109">*It's possible the site appears stuck at **Creating** longer than expected. If more than 24 hours have passed since you first saw this issue, please log a support ticket. In many cases, we're already working on a solution. Please give us at least 24 hours to complete a solution.*</span></span>
