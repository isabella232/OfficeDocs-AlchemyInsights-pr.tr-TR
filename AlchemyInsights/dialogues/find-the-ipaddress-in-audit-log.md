---
title: Denetim günlüğünde IP adresini bulma
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429794"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="cf712-102">Denetim günlüğünde IP adresini bulma</span><span class="sxs-lookup"><span data-stu-id="cf712-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="cf712-103">Kullanıcı veya yönetici tarafından gerçekleştirilen bir etkinlikle ilgili IP adresi denetim günlüklerinde gösterilir.</span><span class="sxs-lookup"><span data-stu-id="cf712-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="cf712-104">İstemci bilgileri de günlüğe kaydedilir.</span><span class="sxs-lookup"><span data-stu-id="cf712-104">The client information is also logged.</span></span> <span data-ttu-id="cf712-105">IP adresini şu şekilde tanımlayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="cf712-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="cf712-106">[Office 365 Güvenlik ve Uyumluluk & gidin.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="cf712-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="cf712-107">Arama **Denetimi günlüğü** arama öğesini  >  **[seçin.](https://go.microsoft.com/fwlink/?linkid=2103759)**</span><span class="sxs-lookup"><span data-stu-id="cf712-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="cf712-108">Denetimi açmamız gereken bir bildirim görüyorsanız, şimdi devam edin ve bu bildirimi açmayın.</span><span class="sxs-lookup"><span data-stu-id="cf712-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="cf712-109">Bu özellik etkinleştirilmemişse, arama sonuçları önceki tarihlerden veri alamayabilecektir.</span><span class="sxs-lookup"><span data-stu-id="cf712-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="cf712-110">Belirli bir etkinlikle ilgileniyorsanız, Etkinlikler listesinden bu **etkinliği** seçin; aksi takdirde, varsayılan olarak seçili kullanıcı için tüm etkinlikler döndürülür.</span><span class="sxs-lookup"><span data-stu-id="cf712-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="cf712-111">Etkinlikler menüsünden belirli etkinliklerin seçiilenem **sağlanamay olabileceğini** unutmayın; bununla birlikte, tüm etkinlikler için sonuçları **göster seçiliyse bu denetim** öğeleri döndürülür (varsayılan ayar).</span><span class="sxs-lookup"><span data-stu-id="cf712-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="cf712-112">Tarih aralığını belirtin ve Kullanıcılar **alanında,** araştırma yapmak istediğiniz kullanıcının kullanıcı adını seçin.</span><span class="sxs-lookup"><span data-stu-id="cf712-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="cf712-113">**Ara'ya seçin.**</span><span class="sxs-lookup"><span data-stu-id="cf712-113">Select **Search**.</span></span> <span data-ttu-id="cf712-114">Etkinlikler Sonuçlar altında **görüntülenir.**</span><span class="sxs-lookup"><span data-stu-id="cf712-114">The activities appear under **Results**.</span></span> <span data-ttu-id="cf712-115">Her etkinliğin IP adresini görebilir.</span><span class="sxs-lookup"><span data-stu-id="cf712-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="cf712-116">Ayrıntıları görüntülemek için bir etkinlik seçin ve ardından Daha Fazla **Bilgi'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="cf712-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="cf712-117">Daha fazla bilgi edinmek için, sık karşılaşılan senaryoların sorunlarını gidermek için [Office 365 denetim günlüğünde aramama bakın.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="cf712-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>