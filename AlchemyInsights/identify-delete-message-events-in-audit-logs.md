---
title: Denetim günlüklerini sil iletisi olayları tanımlama
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 0fb5d6aa0c99f7f68459c40302869bed69583b3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755172"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="2be81-102">Denetim günlükleri silinmiş e-posta iletileri için</span><span class="sxs-lookup"><span data-stu-id="2be81-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="2be81-103">Ocak 2019 içinde başlayarak, posta kutusu denetim günlüğü varsayılan olarak Microsoft açmak.</span><span class="sxs-lookup"><span data-stu-id="2be81-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="2be81-104">Aksi halde, belirli bir kullanıcı için silme iletisi olayları gözden geçirmek için silme eylemleri denetleme için el ile etkinleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="2be81-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="2be81-105">Posta kutusu denetim günlüğü zaten, kuruluşunuz için veya belirli bir kullanıcı için etkin, aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="2be81-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="2be81-106">Oturum [Office 365 güvenlik & Uyumluluk Merkezi](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="2be81-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="2be81-107">**Arama ve araştırma'yı** tıklatın ve **Denetim günlüğü Ara**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="2be81-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="2be81-108">**Başlangıç tarihi** ve **Bitiş tarihi** alanlarında tarih aralığını seçin.</span><span class="sxs-lookup"><span data-stu-id="2be81-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="2be81-109">(Silinmiş öğeleri kullanıcı) incelemek istediğiniz kullanıcının kullanıcı adını belirtin.</span><span class="sxs-lookup"><span data-stu-id="2be81-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="2be81-110">**Silinmiş Öğeler klasöründen silinen iletiler** ve **Silinmiş Öğeler klasörüne Moved iletiler** **Aktiviteler** alanında seçin.</span><span class="sxs-lookup"><span data-stu-id="2be81-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="2be81-111">**Ara**' yı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="2be81-111">Click **Search**.</span></span>

<span data-ttu-id="2be81-112">Sonuçlarda bir denetim kaydı seçin.</span><span class="sxs-lookup"><span data-stu-id="2be81-112">In the results, select an audit record.</span></span> <span data-ttu-id="2be81-113">Ayrıntılar çıkma **Daha fazla Bilgi'yi**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="2be81-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="2be81-114">Silinmiş bir öğeyi (örneğin, konu satırı ve onu silindiğinde öğenin konumunu) hakkında ek bilgi **AffectedItems** alanında görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="2be81-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="2be81-115">**ClientInfoString** özelliği, Outlook, Outlook web (eski adı Outlook Web App bilinir) veya başka bir aygıt silme işlemi oluştu, gösterecektir.</span><span class="sxs-lookup"><span data-stu-id="2be81-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="2be81-116">Daha fazla bilgi için bkz: [belirleme kimin e-posta iletmek için bir posta kutusu ayarlayın](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="2be81-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="2be81-117">**Not**: denetim günlüğü özelliğini kullanarak silinmiş öğeleri geri alamazsınız.</span><span class="sxs-lookup"><span data-stu-id="2be81-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="2be81-118">Outlook Web silinmiş iletileri almak için bkz: [Recover silinmiş öğeleri Outlook Web App'te](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="2be81-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
