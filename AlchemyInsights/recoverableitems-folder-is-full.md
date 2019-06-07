---
title: 1336 RecoverableItems klasörü dolu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: cfcc69c1b3a59c73037d9a493af4ece86b7b7208
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762100"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="a8290-102">Kurtarılabilir öğeleri klasörü dolu</span><span class="sxs-lookup"><span data-stu-id="a8290-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="a8290-103">Office 365'te çevrimiçi Exchange posta kutuları için kurtarılabilir öğeleri klasör için varsayılan depolama sınırı 30 GB'dır.</span><span class="sxs-lookup"><span data-stu-id="a8290-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="a8290-104">Posta kutusu dava tutun, eBulma tutun yerleştirilir veya bir Office 365 bekletme ilkesine atandığından kurtarılabilir öğeleri klasör için depolama sınırı 100 GB'a otomatik olarak artırılır.</span><span class="sxs-lookup"><span data-stu-id="a8290-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>

<span data-ttu-id="a8290-105">Kurtarılabilir öğeleri klasör depolama sınırına ulaştığında, posta kutusu işlevselliği aşağıdaki şekillerde etkilenir:</span><span class="sxs-lookup"><span data-stu-id="a8290-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="a8290-106">Kullanıcının posta kutusundan öğeler silinemiyor.</span><span class="sxs-lookup"><span data-stu-id="a8290-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="a8290-107">Yönetilen Klasör Yardımcısı bekletme etiket veya yönetilen klasör ayarları temel öğelerini silemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="a8290-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="a8290-108">Tek öğe kurtarma etkinleştirilmiş veya beklemeye alınan posta kutuları için kopyası üzerinde yazma sayfa koruma işlemi kullanıcı tarafından düzenlenen öğelerin sürümleri korunamaz.</span><span class="sxs-lookup"><span data-stu-id="a8290-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="a8290-109">Denetim günlüğü etkin posta kutunuz posta kutuları için posta kutusu denetim günlük girdisi denetimleri alt kurtarılabilir öğeler klasörüne kaydedilebilir.</span><span class="sxs-lookup"><span data-stu-id="a8290-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="a8290-110">Beklemede olmayan posta kutuları için admins kullanabilirsiniz `Search-Mailbox -SearchDumpsterOnly -DeleteContent` kurtarılabilir öğeleri klasörü'ndeki öğeleri silmek için Exchange Online PowerShell komutunu.</span><span class="sxs-lookup"><span data-stu-id="a8290-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="a8290-111">Daha fazla bilgi için, aşağıdaki konulara bakın:</span><span class="sxs-lookup"><span data-stu-id="a8290-111">For more information, see the following topics:</span></span> 

- [<span data-ttu-id="a8290-112">Arama ve iletileri silme</span><span class="sxs-lookup"><span data-stu-id="a8290-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="a8290-113">Posta kutusu arama</span><span class="sxs-lookup"><span data-stu-id="a8290-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="a8290-114">Beklemede olan posta kutuları için admins tutma bunlar kurtarılabilir öğeleri klasörden silinen öğeleri için önce kaldırmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="a8290-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="a8290-115">Daha fazla bilgi için bkz: [Klasör bulut tabanlı posta kutularının üzerinde tutun kurtarılabilir öğeleri öğeleri silmek](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="a8290-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="a8290-116">Kurtarılabilir öğeleri klasör tam olmasını önlemek için Yöneticiler kurtarılabilir klasör için posta kutuları üzerinde tutun ve kullanıcının arşive kurtarılabilir Öğeler klasöründeki öğeleri taşıyan bir posta kutusu bekletme ilkesini ayarlamak öğelerin depolama sınırını artırabilirsiniz posta kutusu.</span><span class="sxs-lookup"><span data-stu-id="a8290-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="a8290-117">[Kurtarılabilir öğeleri üzerinde posta kutuları için kota tutun artırmak](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)bakın.</span><span class="sxs-lookup"><span data-stu-id="a8290-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
