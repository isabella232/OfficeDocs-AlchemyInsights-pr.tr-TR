---
title: SharePoint kök sitesini silme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003017"
- "5727"
ms.openlocfilehash: d33029b6fe333b38cee7dba66ba4a5044248f174
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "50714307"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="655c1-102">SharePoint kök sitesini silme</span><span class="sxs-lookup"><span data-stu-id="655c1-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="655c1-103">SharePoint kök sitesini silme  **işlemi desteklenmemektedir.**</span><span class="sxs-lookup"><span data-stu-id="655c1-103">Deleting the SharePoint root site is  **not supported.**</span></span>

1.  <span data-ttu-id="655c1-104">Kök site zaten silinmişse, kullanıcılar siteye erişmeye çalışırken 404 Dosya Bulunamadı hatasıyla deneyimler.</span><span class="sxs-lookup"><span data-stu-id="655c1-104">If the root site has already been deleted, users will experience a  404 File Not Found  error when trying to access the site.</span></span>
2.  <span data-ttu-id="655c1-105">Çözmek için, Silinmiş siteler sayfasına gidip kök siteyi [](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) seçin ve Geri Yükle'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="655c1-105">To resolve, restore the site  from the new SharePoint admin center by going to the  [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  page, select the root site and click  Restore.</span></span>
3.  <span data-ttu-id="655c1-106">Kök siteyi silmek yerine, kök [site geri yüklendiktan](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  sonra yeni SharePoint Yönetim Merkezi'nde siteyi değiştir'i kullanın.</span><span class="sxs-lookup"><span data-stu-id="655c1-106">Instead of deleting the root site, use [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="655c1-107">Daha fazla bilgi için bkz. [Kök sitenizi modernleştirme](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="655c1-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span></span>