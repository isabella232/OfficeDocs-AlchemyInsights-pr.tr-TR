---
title: 2609-tutma-veya-ediscovery-hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994104"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="d78b2-102">SharePoint Online veya OneDrive for Business'taki öğeleri sileme</span><span class="sxs-lookup"><span data-stu-id="d78b2-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="d78b2-103">OneDrive sitesinin SharePoint sitesine veya belirli bir öğeye saklama ilkesi, bekletme etiketi veya eDiscovery tutma uygulandığından siz veya kullanıcılarınız SharePoint Online veya OneDrive for Business'taki öğeleri silemez.</span><span class="sxs-lookup"><span data-stu-id="d78b2-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="d78b2-104">Bu, belge, belge sürümü, klasör, belge kitaplığı, liste, uygulama, site veya site koleksiyonunu silememeyi içerir.</span><span class="sxs-lookup"><span data-stu-id="d78b2-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="d78b2-105">Tutulan bir öğeyi silmeye çalışırsanız alabileceğiniz hata iletilerine bazı örnekler aşağıda verilmiştir:</span><span class="sxs-lookup"><span data-stu-id="d78b2-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="d78b2-106">"Bu site bir eDiscovery tutma veya saklama ilkesine dahil edildiği için silinemez"</span><span class="sxs-lookup"><span data-stu-id="d78b2-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="d78b2-107">"Bu site, silinmesini engellemek için ayarlanmış bir uyumluluk ilkesine sahiptir"</span><span class="sxs-lookup"><span data-stu-id="d78b2-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="d78b2-108">"Bir uyumluluk ilkesi şu anda bu sitenin silinmesini engelliyor"</span><span class="sxs-lookup"><span data-stu-id="d78b2-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="d78b2-109">"Bu site koleksiyonu, eDiscovery tutma veya saklama ilkesine dahil olan siteleri içerdiğinden silinemez"</span><span class="sxs-lookup"><span data-stu-id="d78b2-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="d78b2-110">"Klasörü silmeden önce bu klasördeki tüm öğeleri silmeniz gerekir"</span><span class="sxs-lookup"><span data-stu-id="d78b2-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="d78b2-111">"Beklemede veya bekletme ilkesi nde olduğu için bu öğenin sürümleri silinemez"</span><span class="sxs-lookup"><span data-stu-id="d78b2-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="d78b2-112">"Öğe beklemedeyken silinemez"</span><span class="sxs-lookup"><span data-stu-id="d78b2-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="d78b2-113">"Bu öğeye uygulanan etiket, etiketin düzenlenmesini veya silinmesini engeller"</span><span class="sxs-lookup"><span data-stu-id="d78b2-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="d78b2-114">"Liste beklemede veya bekletme ilkesindeyken silinemez"</span><span class="sxs-lookup"><span data-stu-id="d78b2-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="d78b2-115">"Engellenirse veya bir saklama ilkesi uygulanırsa liste silinemez"</span><span class="sxs-lookup"><span data-stu-id="d78b2-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="d78b2-116">Bu senaryolardan birinde öğeleri silmek için, bekletme ilkesi, bekletme etiketi veya eDiscovery tutmanın kaldırılması gerekir (veya bir sitenin bekletme ilkesinin dışında tutulması gerekir).</span><span class="sxs-lookup"><span data-stu-id="d78b2-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="d78b2-117">Bu soruna neden olan ilgili beklemeyi devre dışı bırakmak veya hariç tutmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="d78b2-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="d78b2-118">Bekletme ilkesi veya tutma kaldırıldıktan sonra, değişikliğin etkili olması 24 saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="d78b2-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="d78b2-119">SharePoint sitelerine ve OneDrive hesaplarına uygulanabilecek farklı saklama ve bekletme özellikleri hakkında bilgi için aşağıdaki konulardan birine bakın.</span><span class="sxs-lookup"><span data-stu-id="d78b2-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="d78b2-120">Bekletme ilkelerine genel bakış</span><span class="sxs-lookup"><span data-stu-id="d78b2-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="d78b2-121">Bekletme etiketlerini genel bakış</span><span class="sxs-lookup"><span data-stu-id="d78b2-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="d78b2-122">Gelişmiş eDiscovery'de tutar'ı yönetme</span><span class="sxs-lookup"><span data-stu-id="d78b2-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="d78b2-123">eDiscovery tutar</span><span class="sxs-lookup"><span data-stu-id="d78b2-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="d78b2-124">Eski site kapatma ve silme ilkeleri</span><span class="sxs-lookup"><span data-stu-id="d78b2-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
