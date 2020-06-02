---
title: Denetim günlüklerinde ileti olaylarını silme'yi tanımlama
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509008"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="fedf7-102">Silinen e-posta iletileri için denetim günlükleri</span><span class="sxs-lookup"><span data-stu-id="fedf7-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="fedf7-103">Ocak 2019'dan itibaren Microsoft varsayılan olarak posta kutusu denetim günlüğe kaydetmeyi açıyor.</span><span class="sxs-lookup"><span data-stu-id="fedf7-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="fedf7-104">Aksi takdirde, belirli bir kullanıcı için ileti olayları silme gözden geçirmek için, denetim için silme eylemleri el ile etkinleştirmek gerekir.</span><span class="sxs-lookup"><span data-stu-id="fedf7-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="fedf7-105">Kuruluşunuz veya belirli bir kullanıcı için posta kutusu denetim günlüğü zaten etkinse, aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="fedf7-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="fedf7-106">[Microsoft 365 Güvenlik & Uyumluluk Merkezi'nde](https://protection.office.com/) oturum açın</span><span class="sxs-lookup"><span data-stu-id="fedf7-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="fedf7-107">**Arama ve Araştırma'yı** tıklatın ve **Denetim Günlüğü Arama'yı**seçin.</span><span class="sxs-lookup"><span data-stu-id="fedf7-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="fedf7-108">**Başlangıç tarihi** ve Bitiş **tarihi** alanlarındaki tarih aralığını seçin.</span><span class="sxs-lookup"><span data-stu-id="fedf7-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="fedf7-109">Araştırmak istediğiniz kullanıcı (öğeleri silen kullanıcı) için kullanıcı adı belirtin.</span><span class="sxs-lookup"><span data-stu-id="fedf7-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="fedf7-110">**Etkinlikler** alanında, **Silinmiş Öğeler klasöründen Silinmiş iletileri** ve **Silinmiş Öğeler klasörüne taşınan iletileri**seçin.</span><span class="sxs-lookup"><span data-stu-id="fedf7-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="fedf7-111">**Arama'yı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="fedf7-111">Click **Search**.</span></span>

<span data-ttu-id="fedf7-112">Sonuçlarda, bir denetim kaydı seçin.</span><span class="sxs-lookup"><span data-stu-id="fedf7-112">In the results, select an audit record.</span></span> <span data-ttu-id="fedf7-113">Ayrıntılarflyout, daha **fazla bilgi**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="fedf7-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="fedf7-114">Silinen öğe yle ilgili ek bilgiler (örneğin, konu satırı ve silindiğinde öğenin konumu) **Etkilenen Öğeler** alanında görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="fedf7-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="fedf7-115">**ClientInfoString** özelliği silme outlook, Outlook web (eski Outlook Web App olarak da bilinir) veya başka bir aygıtta oluştu gösterir.</span><span class="sxs-lookup"><span data-stu-id="fedf7-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="fedf7-116">Daha fazla bilgi için [bkz.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)</span><span class="sxs-lookup"><span data-stu-id="fedf7-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="fedf7-117">**Not**: Denetim günlüğü özelliğini kullanarak silinen öğeleri alamazsınız.</span><span class="sxs-lookup"><span data-stu-id="fedf7-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="fedf7-118">Web'de Outlook'ta silinen iletileri almak için [bkz.](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)</span><span class="sxs-lookup"><span data-stu-id="fedf7-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
