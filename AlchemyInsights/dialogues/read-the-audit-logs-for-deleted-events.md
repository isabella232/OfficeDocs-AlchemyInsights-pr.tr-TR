---
title: Silinen olayların denetim günlüklerini okuma
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429819"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="f3460-102">Silinen olayların denetim günlüklerini okuma</span><span class="sxs-lookup"><span data-stu-id="f3460-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="f3460-103">Bunu şu şekilde yapacaksınız:</span><span class="sxs-lookup"><span data-stu-id="f3460-103">Here's how to do this:</span></span>

1. <span data-ttu-id="f3460-104">[Office 365 Güvenlik ve Uyumluluk & gidin.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="f3460-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="f3460-105">Arama **Denetimi günlüğü** arama öğesini  >  [**seçin.**](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="f3460-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="f3460-106">Özelliği açmak için ihtiyacınız olduğunu fark ediyorsanız, şimdi devam edin ve özelliği açabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f3460-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="f3460-107">Özellik açık değilse, arama sonuçları önceki tarihlerden veri alamı olmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="f3460-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="f3460-108">**Etkinlikler'i** seçin ve **ardından Exchange posta kutusu etkinliklerini bulun.**</span><span class="sxs-lookup"><span data-stu-id="f3460-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="f3460-109">Silinmiş Öğeler **klasöründeki Silinmiş iletiler ve** İletiler **Silinmiş Öğeler klasör seçeneklerine** taşındı seçeneklerini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="f3460-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="f3460-110">Bitir bittiğinde, Etkinlikler bölmesini simge durumuna küçültmek için **bölmenin dışına** tıklayın.</span><span class="sxs-lookup"><span data-stu-id="f3460-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="f3460-111">Tarih aralığını belirtin ve Kullanıcılar  kutusunda araştırma yapmak istediğiniz kullanıcının kullanıcı adını seçin.</span><span class="sxs-lookup"><span data-stu-id="f3460-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="f3460-112">Bir defada birden çok kullanıcı seçin.</span><span class="sxs-lookup"><span data-stu-id="f3460-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="f3460-113">**Ara'ya seçin.**</span><span class="sxs-lookup"><span data-stu-id="f3460-113">Select **Search**.</span></span> <span data-ttu-id="f3460-114">Etkinlikler Sonuçlar altında **görüntülenir.**</span><span class="sxs-lookup"><span data-stu-id="f3460-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="f3460-115">Ayrıntıları görüntülemek için bir etkinlik seçin ve ardından Daha Fazla **Bilgi'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="f3460-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="f3460-116">Silinen öğe hakkında konu satırı ve silindiğinde öğenin konumu gibi ek bilgiler **AffectedItems alanında** görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="f3460-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="f3460-117">Denetim günlüğü özelliğini kullanarak silinmiş öğeleri geri yükleyemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="f3460-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="f3460-118">Silinmiş öğeleri geri yüklemek için, Outlook [Web App'te silinmiş öğeleri veya e-postayı kurtarma'ya bakın.](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="f3460-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="f3460-119">Daha fazla bilgi edinmek için, sık karşılaşılan senaryoların sorunlarını gidermek için [Office 365 denetim günlüğünde aramama bakın.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="f3460-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
