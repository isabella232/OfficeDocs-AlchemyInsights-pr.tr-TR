---
title: 1336 RecoverableItems klasörü dolu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720272"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="802cd-102">Kurtarılabilir Öğeler klasörü dolu</span><span class="sxs-lookup"><span data-stu-id="802cd-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="802cd-103">Exchange Online posta kutuları için, Kurtarılabilir Öğeler klasörü için varsayılan depolama sınırı 30 GB'dır.</span><span class="sxs-lookup"><span data-stu-id="802cd-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="802cd-104">Kurtarılabilir Öğeler klasörü için depolama sınırı, posta kutusu Dava Bekletme, eDiscovery tutma veya saklama ilkesine atanmışsa otomatik olarak 100 GB'a yükseltilir.</span><span class="sxs-lookup"><span data-stu-id="802cd-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="802cd-105">Kurtarılabilir Öğeler klasörü depolama sınırına ulaştığında, posta kutusu işlevselliği aşağıdaki şekillerde etkilenir:</span><span class="sxs-lookup"><span data-stu-id="802cd-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="802cd-106">Kullanıcı öğeleri posta kutusundan silemez.</span><span class="sxs-lookup"><span data-stu-id="802cd-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="802cd-107">Yönetilen Klasör Yardımcısı, bekletme etiketine veya yönetilen klasör ayarlarına göre öğeleri silemez.</span><span class="sxs-lookup"><span data-stu-id="802cd-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="802cd-108">Tek Öğe Kurtarma özelliği etkinleştirilmiş veya beklemeye alınan posta kutuları için, yazma da yazma sayfası koruma işlemi, kullanıcı tarafından düzenlenen öğelerin sürümlerini koruyamaz.</span><span class="sxs-lookup"><span data-stu-id="802cd-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="802cd-109">Posta kutusu denetim günlüğü etkinleştirilmiş posta kutuları için, Kurtarılabilir Öğeler klasöründeki Denetimler alt klasörüne hiçbir posta kutusu denetim günlüğü girişi kaydedilemez.</span><span class="sxs-lookup"><span data-stu-id="802cd-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="802cd-110">Beklemede olmayan posta kutularında yöneticiler, Kurtarılabilir `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Öğeler klasöründeki öğeleri silmek için Exchange Online PowerShell'deki komutu kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="802cd-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="802cd-111">Daha fazla bilgi için, aşağıdaki konulara bakın:</span><span class="sxs-lookup"><span data-stu-id="802cd-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="802cd-112">İletileri arama ve silme</span><span class="sxs-lookup"><span data-stu-id="802cd-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="802cd-113">Arama-Posta Kutusu</span><span class="sxs-lookup"><span data-stu-id="802cd-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="802cd-114">Beklemede olan posta kutuları için, yöneticilerin öğeleri Kurtarılabilir Öğeler klasöründen silmeden önce beklemeyi kaldırmaları gerekir.</span><span class="sxs-lookup"><span data-stu-id="802cd-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="802cd-115">Daha fazla bilgi için [bkz.](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)</span><span class="sxs-lookup"><span data-stu-id="802cd-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="802cd-116">Kurtarılabilir Öğeler klasörünün dolmasını önlemeye yardımcı olmak için yöneticiler, bekleyen posta kutuları için Kurtarılabilir Öğeler klasörünün depolama sınırını artırabilir ve öğeleri Kurtarılabilir Öğeler klasöründen kullanıcının arşiv posta kutusuna taşıyan bir posta kutusu bekletme ilkesi ayarlayabilir.</span><span class="sxs-lookup"><span data-stu-id="802cd-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="802cd-117">Bkz. [Beklemedeki posta kutuları için Kurtarılabilir Öğeler kotasını artırın.](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)</span><span class="sxs-lookup"><span data-stu-id="802cd-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
