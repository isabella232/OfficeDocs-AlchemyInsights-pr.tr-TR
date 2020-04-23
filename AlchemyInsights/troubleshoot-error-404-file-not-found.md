---
title: Sorun Giderme Hatası 404, Dosya bulunamadı
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: ed35c790dfb048aa6f33fa439b7636864a6e6e6c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759784"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="215fa-102">Sorun Giderme Hatası 404, Dosya bulunamadı</span><span class="sxs-lookup"><span data-stu-id="215fa-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="215fa-103">Kullanıcılar SharePoint veya OneDrive'da bir siteye veya dosyaya erişmeye çalışırken bir Hata 404 alınır.</span><span class="sxs-lookup"><span data-stu-id="215fa-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="215fa-104">Bunun nedeni genellikle bir site nin veya dosyanın veya grubun yeniden adlandırılsa, taşınmasından veya silinmekten kaynaklanır.</span><span class="sxs-lookup"><span data-stu-id="215fa-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="215fa-105">Örneğin: Kullanıcılar Kök Site Koleksiyonu'na erişmeye çalışan bir 404 Hatası yla karşılaşır ve silinmiştir.</span><span class="sxs-lookup"><span data-stu-id="215fa-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="215fa-106">Yeniden adlandırılmış, taşınmış veya silinmiş bir Site için Hata 404'ün çözüme kavuşturulması için:</span><span class="sxs-lookup"><span data-stu-id="215fa-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="215fa-107">Klasik Yönetici Merkezi'nde bulunan klasik siteler için [silinmiş site koleksiyonunu geri yükle'ye](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)bakın.</span><span class="sxs-lookup"><span data-stu-id="215fa-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="215fa-108">Yeni SharePoint yönetici merkezinde bulunan modern siteler (iletişim, gruba bağlı veya diğer siteler) için, [yeni SharePoint yönetici merkezinde silinen siteleri görüntüle ve geri yükleyin.](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)</span><span class="sxs-lookup"><span data-stu-id="215fa-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="215fa-109">Yeniden adlandırılmış, taşınmış veya silinmiş bir Dosya (veya başka bir öğe) için Hata 404'ü çözmek için:</span><span class="sxs-lookup"><span data-stu-id="215fa-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="215fa-110">SharePoint veya OneDrive sitesine gidin ve Site içeriğinden Geri Dönüşüm Kutusu'nu görüntüleyin.</span><span class="sxs-lookup"><span data-stu-id="215fa-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="215fa-111">Bkz. [SharePoint sitesinin Geri Dönüşüm Kutusu'ndaki öğeleri geri yükleme.](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online)</span><span class="sxs-lookup"><span data-stu-id="215fa-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="215fa-112">Öğeyi hala bulamıyorsanız, günlük kaydı etkinse denetim günlüğün [&de](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c)arama yapabilirsiniz bkz.</span><span class="sxs-lookup"><span data-stu-id="215fa-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Microsoft 365 Security & Compliance Center](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c).</span></span>
