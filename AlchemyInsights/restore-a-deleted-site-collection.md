---
title: Silinmiş bir site koleksiyonunu geri yükleme
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 1f9a66daf7bee43291b785b6260aec8725ee782f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753806"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="7daa4-102">Silinmiş bir site koleksiyonunu geri yükleme</span><span class="sxs-lookup"><span data-stu-id="7daa4-102">Restore a deleted site collection</span></span>

<span data-ttu-id="7daa4-103">Bir yönetici Klasik site koleksiyonu silmesinden burada kalıcı olarak silinmeden önce 93 gün tutulan Dönüşüm, site koleksiyonundaki yerleştirilir.</span><span class="sxs-lookup"><span data-stu-id="7daa4-103">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="7daa4-104">Site koleksiyonu geri yüklemek için:</span><span class="sxs-lookup"><span data-stu-id="7daa4-104">To restore the site collection:</span></span>
  
1. <span data-ttu-id="7daa4-105">Klasik SharePoint Yönetim Merkezi'nde Şerit üzerinde **Geri Dönüşüm Kutusu'nu** tıklatın.</span><span class="sxs-lookup"><span data-stu-id="7daa4-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="7daa4-106">Geri yüklemek istediğiniz site koleksiyonunu yanındaki onay kutusunu seçin.</span><span class="sxs-lookup"><span data-stu-id="7daa4-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="7daa4-107">**Silinen öğeleri geri yükle**' yi tıklatın.</span><span class="sxs-lookup"><span data-stu-id="7daa4-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="7daa4-108">Silinen iletişim site geri yüklemek için yeni SharePoint Yönetim Merkezi önizleme özelliğini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7daa4-108">To restore a deleted communication site, you can use the new SharePoint admin center preview.</span></span> <span data-ttu-id="7daa4-109">Aksi takdirde, PowerShell kullanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="7daa4-109">Otherwise, you need to use PowerShell.</span></span> <span data-ttu-id="7daa4-110">Bir Office 365 grubuna ait bir siteyi geri yüklemek için Exchange Yönetim Merkezi grubunda geri gerekir.</span><span class="sxs-lookup"><span data-stu-id="7daa4-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="7daa4-111">Bunlar silinmiş sonraki 30 gün için grupları geri yüklenebilir.</span><span class="sxs-lookup"><span data-stu-id="7daa4-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

