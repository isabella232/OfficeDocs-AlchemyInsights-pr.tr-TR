---
title: Silinen bir siteyi geri yükleme
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: edf851da951e163f30660d524049abe0798a8314
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048816"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="660e9-102">Silinen bir siteyi geri yükleme</span><span class="sxs-lookup"><span data-stu-id="660e9-102">Restore a deleted site</span></span>

<span data-ttu-id="660e9-103">Bir yönetici Bir SharePoint sitesini sildiğinde, site koleksiyonugeri dönüşüm kutusuna yerleştirilir ve kalıcı olarak silinmeden önce 93 gün boyunca saklanır.</span><span class="sxs-lookup"><span data-stu-id="660e9-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="660e9-104">Siteyi geri yüklemek için:</span><span class="sxs-lookup"><span data-stu-id="660e9-104">To restore the site:</span></span>
  
1. <span data-ttu-id="660e9-105">Yeni SharePoint yönetici merkezinde, şeritteki **Geri Dönüşüm Kutusu'nu** tıklatın.</span><span class="sxs-lookup"><span data-stu-id="660e9-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="660e9-106">Geri yüklemek istediğiniz site koleksiyonunun yanındaki onay kutusunu seçin.</span><span class="sxs-lookup"><span data-stu-id="660e9-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="660e9-107">**Silinen Öğeleri Geri Yükle'yi**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="660e9-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="660e9-108">Silinen bir iletişim sitesini geri yüklemek için yeni SharePoint yönetici merkezini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="660e9-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="660e9-109">Aksi takdirde, Microsoft PowerShell kullanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="660e9-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="660e9-110">Office 365 grubuna ait bir siteyi geri yüklemek için, grubu Exchange yönetici merkezindeki geri yüklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="660e9-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="660e9-111">Gruplar silindikten sonra 30 gün boyunca geri yüklenebilir.</span><span class="sxs-lookup"><span data-stu-id="660e9-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

