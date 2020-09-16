---
title: Sorun giderme 404, dosya bulunamadı
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: e76864949bde7230e63f509823ab1e3edf631388
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750111"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="acb58-102">Sorun giderme 404, dosya bulunamadı</span><span class="sxs-lookup"><span data-stu-id="acb58-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="acb58-103">Kullanıcılar SharePoint veya OneDrive 'da bir siteye veya dosyaya erişmeye çalıştığında bir 404 hatası alındı.</span><span class="sxs-lookup"><span data-stu-id="acb58-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="acb58-104">Bunun nedeni genellikle site veya dosya veya grubun yeniden adlandırılmasına, taşınmasına veya silinmesine neden olur.</span><span class="sxs-lookup"><span data-stu-id="acb58-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="acb58-105">Örneğin: kullanıcılar kök site koleksiyonuna erişmeye çalışırken bir 404 hatası yaşayacaktır.</span><span class="sxs-lookup"><span data-stu-id="acb58-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="acb58-106">Yeniden adlandırılan, taşınan veya silinen bir sitenin 404 hatasını çözmek için:</span><span class="sxs-lookup"><span data-stu-id="acb58-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="acb58-107">Klasik Yönetim merkezinde bulunan klasik siteler için, [Silinmiş bir site koleksiyonunu geri yükleme](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="acb58-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="acb58-108">Yeni SharePoint Yönetim merkezinde bulunan modern siteler (iletişim, Grup bağlı veya diğer siteler) için, [Yeni SharePoint Yönetim merkezinde silinen siteleri görüntüleme ve geri yükleme](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="acb58-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="acb58-109">Yeniden adlandırılan, taşınan veya silinen bir dosyanın (veya başka bir öğenin) 404 hatasını çözmek için:</span><span class="sxs-lookup"><span data-stu-id="acb58-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="acb58-110">SharePoint veya OneDrive sitesine gidin ve site içeriğinden geri dönüşüm kutusunu görüntüleyin.</span><span class="sxs-lookup"><span data-stu-id="acb58-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="acb58-111">[SharePoint sitesinin geri dönüşüm kutusu 'ndaki öğeleri](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online)görün.</span><span class="sxs-lookup"><span data-stu-id="acb58-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="acb58-112">Öğeyi yine de bulamıyorsanız, günlük etkinse denetim günlüğünde arama yapabilirsiniz [kutusunda, Microsoft 365 güvenlik & Uyumluluk Merkezi 'nde denetim günlüğünde arama](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)yapın.</span><span class="sxs-lookup"><span data-stu-id="acb58-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Microsoft 365 Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>
