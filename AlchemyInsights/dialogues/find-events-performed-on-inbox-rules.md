---
title: Gelen kutusu kurallarında gerçekleştirilen olayları bulma
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430310"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="e2039-102">Gelen kutusu kurallarında gerçekleştirilen olayları bulma</span><span class="sxs-lookup"><span data-stu-id="e2039-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="e2039-103">Gelen kutusu kuralları oluşturulduğunda, değiştirdiğinde veya silindiğinde olaylar denetim günlüğüne kaydedilir.</span><span class="sxs-lookup"><span data-stu-id="e2039-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="e2039-104">Bunları şu şekilde gözden geçirsiniz:</span><span class="sxs-lookup"><span data-stu-id="e2039-104">Here's how to review them:</span></span>

1. <span data-ttu-id="e2039-105">[Office 365 Güvenlik ve Uyumluluk & gidin.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="e2039-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="e2039-106">Denetim günlüğü > Arama'ya seçin.</span><span class="sxs-lookup"><span data-stu-id="e2039-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e2039-107">Denetimi açmamız gereken bir bildirim görüyorsanız, şimdi devam edin ve bu bildirimi açmayın.</span><span class="sxs-lookup"><span data-stu-id="e2039-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="e2039-108">Bu özellik açık değilse, arama sonuçları önceki tarihlerden veri alamı olmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="e2039-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="e2039-109">Etkinlikler alanını seçin, Exchange posta kutusu etkinliklerini bulun ve ardından Outlook Web App'New-InboxRule gelen kutusu kuralı oluştur'u seçin.</span><span class="sxs-lookup"><span data-stu-id="e2039-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="e2039-110">Bitir bittiğinde, Etkinlikler bölmesini simge durumuna küçültmek için bölmenin dışına tıklayın.</span><span class="sxs-lookup"><span data-stu-id="e2039-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="e2039-111">Tarih aralığını belirtin ve Kullanıcılar alanında, araştırma yapmak istediğiniz kullanıcının kullanıcı adını seçin.</span><span class="sxs-lookup"><span data-stu-id="e2039-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="e2039-112">Bir defada birden çok kullanıcı seçin.</span><span class="sxs-lookup"><span data-stu-id="e2039-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="e2039-113">Ara'ya seçin.</span><span class="sxs-lookup"><span data-stu-id="e2039-113">Select Search.</span></span> <span data-ttu-id="e2039-114">Etkinlikler Sonuçlar altında görünür.</span><span class="sxs-lookup"><span data-stu-id="e2039-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="e2039-115">Ayrıntıları görüntülemek için bir etkinlik seçin ve ardından Daha Fazla Bilgi'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="e2039-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="e2039-116">Parametreler bölümünün altında kuralın adını, ayarlanmış koşulları ve kuralın gerçekleştirecek eylemlerini bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e2039-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="e2039-117">Daha fazla bilgi edinmek için bkz. Yaygın senaryoların sorunlarını gidermek için Office 365 denetim günlüğünde arama yapın.</span><span class="sxs-lookup"><span data-stu-id="e2039-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>