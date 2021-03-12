---
title: Bu siteye ulaşamadı- tarayıcıdan veya Teams'den SharePoint sitesine erişmeye çalışırken hata oluştu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005378"
- "9266"
ms.openlocfilehash: 451544fb85522e0eececc9274825805699685ee9
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747035"
---
# <a name="this-site-cant-be-reached-error-when-trying-to-access-sharepoint-site-from-browser-or-teams"></a><span data-ttu-id="671f0-102">Tarayıcıdan veya Teams'den SharePoint sitesine erişmeye çalışırken "Bu siteye erişene yok" hatası</span><span class="sxs-lookup"><span data-stu-id="671f0-102">“This site can’t be reached” error when trying to access SharePoint site from browser or Teams</span></span>

<span data-ttu-id="671f0-103">Tarayıcıdan veya Teams'den SharePoint sitesine erişmeye çalışırken kullanıcılar "Bu siteye erişilene ulaşıla değil" hatasını alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="671f0-103">Users might receive "This site can't be reached" error when trying to access SharePoint site from browser or Teams.</span></span> 

<span data-ttu-id="671f0-104">Bu sorunu çözmek için:</span><span class="sxs-lookup"><span data-stu-id="671f0-104">To resolve this issue:</span></span> 

1. <span data-ttu-id="671f0-105">Giriş sayfasının Geri Dönüşüm kutusu mu yoksa ikinci aşama geri dönüşüm kutusu mu olduğunu kontrol edin ve sayfayı geri yüklenin.</span><span class="sxs-lookup"><span data-stu-id="671f0-105">Check if the home page is in Recycle bin or second-stage recycle bin and restore the page.</span></span>

<span data-ttu-id="671f0-106">**Geri dönüşüm kutusu için doğrudan örnek URL:**https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="671f0-106">**Sample direct URL to recycle bin**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>

1. <span data-ttu-id="671f0-107">Giriş sayfası geri dönüşüm kutusuyla kalıcı olarak kaldırılırsa, Site Sayfaları kitaplığından yeni bir site sayfası oluşturun ve bunu bir giriş sayfası yapın.</span><span class="sxs-lookup"><span data-stu-id="671f0-107">If the home page is permanently removed from the recycle bin, create a new site page from the Site Pages library and make it a homepage.</span></span> 

<span data-ttu-id="671f0-108">**Örnek doğrudan URL:**https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="671f0-108">**Sample direct URL**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>