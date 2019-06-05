---
title: Silinmiş bir dosya veya klasörü geri yüklemek
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: d5250d75a982c0afc9d3e1b2a43be2ba9c3e8f59
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716526"
---
## <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="fa3b9-102">Silinmiş bir dosya veya klasörü geri yüklemek</span><span class="sxs-lookup"><span data-stu-id="fa3b9-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="fa3b9-103">SharePoint çevrimiçi gerçek silme ötesinde ek 14 gün için tüm içeriğini yedeklerini korur.</span><span class="sxs-lookup"><span data-stu-id="fa3b9-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="fa3b9-104">Geri Dönüşüm Kutusu'nu veya dosyaları geri içeriği geri yüklenemez, yönetici Microsoft 14 gün penceresi içinde herhangi bir zamanda geri istemek için Support başvurabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fa3b9-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="fa3b9-105">Yedeklerden geri yüklemeler için site koleksiyonu veya belirli dosyaları, listeler veya kitaplıklar için alt siteler yalnızca tamamlanabilir.</span><span class="sxs-lookup"><span data-stu-id="fa3b9-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="fa3b9-106">SharePoint'ten bir öğe veya siteyi sildiğinizde, hemen kaldırılmaz.</span><span class="sxs-lookup"><span data-stu-id="fa3b9-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="fa3b9-107">Silinmiş öğeleri Geri Dönüşüm Kutusu'na, bir süre için gidin.</span><span class="sxs-lookup"><span data-stu-id="fa3b9-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="fa3b9-108">Bu sırada, sildiğiniz öğeleri özgün konumlarına geri yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fa3b9-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="fa3b9-109">Daha fazla bilgi için aşağıdaki bağlantıları ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="fa3b9-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="fa3b9-110">[SharePoint sitesi Geri Dönüşüm Kutusu'ndaki öğeleri geri yüklemek](https://support.office.com/en-us/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="fa3b9-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/en-us/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

[<span data-ttu-id="fa3b9-111">Silinen dosya veya klasörler OneDrive, geri yükleme</span><span class="sxs-lookup"><span data-stu-id="fa3b9-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/en-us/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="fa3b9-112">Silinmiş bir site koleksiyonu (grup da dahil olmak üzere, iletişim ve diğer siteler) geri yükleme</span><span class="sxs-lookup"><span data-stu-id="fa3b9-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="fa3b9-113">Silinen bir OneDrive sitesini geri yükle</span><span class="sxs-lookup"><span data-stu-id="fa3b9-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/en-us/onedrive/restore-deleted-onedrive)

<span data-ttu-id="fa3b9-114">Toplu Geri Dönüşüm Kutusu'nu eylemler için yöneticileri [Sharepoint çevrimiçi PNP](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)kullanarak düşünebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fa3b9-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

## <a name="files-restore-feature"></a><span data-ttu-id="fa3b9-115">Dosyaları geri yükleme özelliği</span><span class="sxs-lookup"><span data-stu-id="fa3b9-115">Files Restore feature</span></span>

<span data-ttu-id="fa3b9-116">Çok fazla OneDrive veya Sharepoint dosyalarınızı silinmiş, üzerine, bozuk veya kötü amaçlı yazılımın bulaşmış, tüm OneDrive veya Sharepoint kitaplığı dosyaları geri yükleme özelliğini kullanarak önceki bir zamana geri yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fa3b9-116">If lots of your OneDrive or Sharepoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or Sharepoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="fa3b9-117">Geri OneDrive kitaplığı</span><span class="sxs-lookup"><span data-stu-id="fa3b9-117">Restore a OneDrive library</span></span>](https://support.office.com/en-us/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="fa3b9-118">Bir belge kitaplığına geri yükleme</span><span class="sxs-lookup"><span data-stu-id="fa3b9-118">Restore a Document library</span></span>](https://support.office.com/en-us/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a?ui=en-US&amp;rs=en-US&amp;ad=US.)

