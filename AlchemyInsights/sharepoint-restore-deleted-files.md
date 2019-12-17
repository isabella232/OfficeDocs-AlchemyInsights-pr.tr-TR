---
title: Silinen bir dosyayı veya klasörü geri yükleme
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 2702837bff2c0a465dde2c090a44e02747cc85ec
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051085"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="6a11d-102">Silinen bir dosyayı veya klasörü geri yükleme</span><span class="sxs-lookup"><span data-stu-id="6a11d-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="6a11d-103">SharePoint Online, tüm içeriğin yedeklerini gerçek silme işleminin ötesinde 14 gün boyunca saklar.</span><span class="sxs-lookup"><span data-stu-id="6a11d-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="6a11d-104">İçerik Geri Dönüşüm Kutusu veya Dosyaları Geri Yükleme yoluyla geri yüklenemezse, yönetici 14 günlük süre içinde herhangi bir zamanda geri yükleme isteğinde bulunmak için Microsoft Destek'e başvurabilir.</span><span class="sxs-lookup"><span data-stu-id="6a11d-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="6a11d-105">Yedeklemelerden geri yüklemeler yalnızca site koleksiyonları veya alt siteler için tamamlanabilir, belirli dosyalar, listeler veya kitaplıklar için değil.</span><span class="sxs-lookup"><span data-stu-id="6a11d-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="6a11d-106">Bir öğeyi veya siteyi Sharepoint'ten sildiğinizde, öğe hemen kaldırılmaz.</span><span class="sxs-lookup"><span data-stu-id="6a11d-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="6a11d-107">Silinen öğeler bir süre için geri dönüşüm kutusuna gider.</span><span class="sxs-lookup"><span data-stu-id="6a11d-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="6a11d-108">Bu süre zarfında, sildiğiniz öğeleri özgün konumlarına geri yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6a11d-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="6a11d-109">Daha fazla bilgi için lütfen aşağıdaki bağlantıları ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="6a11d-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="6a11d-110">[SharePoint sitesinin Geri Dönüşüm Kutusu'ndaki öğeleri geri yükleyin.](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b)</span><span class="sxs-lookup"><span data-stu-id="6a11d-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="6a11d-111">OneDrive'da silinen dosyaları veya klasörleri geri yükleme</span><span class="sxs-lookup"><span data-stu-id="6a11d-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="6a11d-112">Silinen bir site koleksiyonunu geri yükleme (grup, iletişim ve diğer siteler dahil)</span><span class="sxs-lookup"><span data-stu-id="6a11d-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="6a11d-113">Silinen onedrive sitesini geri yükleme</span><span class="sxs-lookup"><span data-stu-id="6a11d-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="6a11d-114">Toplu geri dönüşüm kutusu eylemleri için, yöneticiler [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)kullanmayı düşünebilir.</span><span class="sxs-lookup"><span data-stu-id="6a11d-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="6a11d-115">**Dosyaları Geri Yükleme özelliği**</span><span class="sxs-lookup"><span data-stu-id="6a11d-115">**Files Restore feature**</span></span>

<span data-ttu-id="6a11d-116">OneDrive veya SharePoint dosyalarınızın çoğu silinirse, üzerine yazılırsa, bozulursa veya kötü amaçlı yazılımlar tarafından enfekte olursa, dosyaların geri yükleme özelliğini kullanarak OneDrive veya SharePoint kitaplığınızın tamamını önceki bir zamana geri yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6a11d-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="6a11d-117">OneDrive kitaplığını geri yükleme</span><span class="sxs-lookup"><span data-stu-id="6a11d-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="6a11d-118">Belge kitaplığını geri yükleme</span><span class="sxs-lookup"><span data-stu-id="6a11d-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

