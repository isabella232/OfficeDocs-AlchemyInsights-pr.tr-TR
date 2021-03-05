---
title: Posta kutusunda kimlerin iletmeyi ayarlay olduğunu ve nasıl olduğunu bulma
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483357"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="994e7-102">Posta kutusunda kimlerin iletmeyi ayarlay hazır olduğunu ve nasıl olduğunu bulma</span><span class="sxs-lookup"><span data-stu-id="994e7-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="994e7-103">Posta kutusunda dış iletme ayarlanmışsa, etkinlik bir posta kutusu cmdlet'i Set-Mailbox denetlenr.</span><span class="sxs-lookup"><span data-stu-id="994e7-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="994e7-104">Denetim günlüğünde etkinliği şu şekilde bulabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="994e7-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="994e7-105">[Office 365 Güvenlik ve Uyumluluk & gidin.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="994e7-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="994e7-106">Arama **Denetimi günlüğü** arama öğesini >  **seçin.**</span><span class="sxs-lookup"><span data-stu-id="994e7-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="994e7-107">Denetimi açmamız gereken bir bildirim görüyorsanız, şimdi devam edin ve bu bildirimi açmayın.</span><span class="sxs-lookup"><span data-stu-id="994e7-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="994e7-108">Bu özellik açık değilse, arama sonuçları önceki tarihlerden veri alamı olmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="994e7-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="994e7-109">Etkinlikler **alanı, tüm etkinlikler** için sonuçları göster **(varsayılan) olarak** ayarlanmış olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="994e7-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="994e7-110">Tarih aralığını belirtin.</span><span class="sxs-lookup"><span data-stu-id="994e7-110">Specify the date range.</span></span> <span data-ttu-id="994e7-111">Kullanıcı adı belirtmenize gerek yok.</span><span class="sxs-lookup"><span data-stu-id="994e7-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="994e7-112">**Ara'ya seçin.**</span><span class="sxs-lookup"><span data-stu-id="994e7-112">Select **Search**.</span></span> <span data-ttu-id="994e7-113">Etkinlikler Sonuçlar altında **görüntülenir.**</span><span class="sxs-lookup"><span data-stu-id="994e7-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="994e7-114">Sonuçları **Filtrele'yi** seçin ve ardından Etkinlik filtresi alanına **Set-mailbox** girin. </span><span class="sxs-lookup"><span data-stu-id="994e7-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="994e7-115">Bu, tüm **Posta Kutusu Kümesi etkinliklerini** döndürür.</span><span class="sxs-lookup"><span data-stu-id="994e7-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="994e7-116">Ayrıntıları görüntülemek için bir etkinlik seçin ve ardından Daha Fazla **Bilgi'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="994e7-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="994e7-117">**Parametreler'in** altında, posta kutusunda ayarlanmış olan iletme e-posta adresini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="994e7-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="994e7-118">**UserID,** posta kutusunda dış iletmeyi ayar eden kullanıcıyı temsil eder.</span><span class="sxs-lookup"><span data-stu-id="994e7-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="994e7-119">Daha fazla bilgi edinmek için, sık karşılaşılan senaryoların sorunlarını gidermek için [Office 365 denetim günlüğünde aramama bakın.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="994e7-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>