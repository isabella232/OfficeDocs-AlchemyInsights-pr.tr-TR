---
title: Denetim günlüklerinde ileti etkinliklerini silme
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696533"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="62ff4-102">Silinen e-posta iletilerinin günlüklerini denetleme</span><span class="sxs-lookup"><span data-stu-id="62ff4-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="62ff4-103">2019 Ocak tarihinde başlayarak varsayılan olarak posta kutusu denetim günlüğü açılıyor.</span><span class="sxs-lookup"><span data-stu-id="62ff4-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="62ff4-104">Başka türlü, belirli bir kullanıcının ileti etkinliklerini gözden geçirmek için, denetim için silme eylemlerini el ile etkinleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="62ff4-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="62ff4-105">Kuruluşunuz için posta kutusu denetim günlüğü zaten etkinleştirilmişse veya belirli bir kullanıcı için aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="62ff4-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="62ff4-106">[Microsoft 365 güvenlik & Uyumluluk Merkezi](https://protection.office.com/) 'nde oturum açma</span><span class="sxs-lookup"><span data-stu-id="62ff4-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="62ff4-107">**Arama ve araştırma** 'ya tıklayın ve **Denetim günlüğü araması**'nı seçin.</span><span class="sxs-lookup"><span data-stu-id="62ff4-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="62ff4-108">**Başlangıç tarihi** ve **bitiş tarihi** alanlarında tarih aralığını seçin.</span><span class="sxs-lookup"><span data-stu-id="62ff4-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="62ff4-109">Araştırmak istediğiniz kullanıcı için Kullanıcı adını belirtin (öğeleri silmiş olan Kullanıcı).</span><span class="sxs-lookup"><span data-stu-id="62ff4-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="62ff4-110">**Etkinlikler** alanında, **Silinmiş Öğeler klasöründen silinmiş iletiler** 'ı seçin ve **iletileri Silinmiş Öğeler klasörüne taşındı**.</span><span class="sxs-lookup"><span data-stu-id="62ff4-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="62ff4-111">**Ara**'ya tıklayın.</span><span class="sxs-lookup"><span data-stu-id="62ff4-111">Click **Search**.</span></span>

<span data-ttu-id="62ff4-112">Sonuçlarda bir denetim kaydı seçin.</span><span class="sxs-lookup"><span data-stu-id="62ff4-112">In the results, select an audit record.</span></span> <span data-ttu-id="62ff4-113">Ayrıntılar açılır listesinde, **ek bilgi**'yi tıklatın.</span><span class="sxs-lookup"><span data-stu-id="62ff4-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="62ff4-114">Silinmiş öğe hakkındaki ek bilgileri (örneğin, konu satırı ve silindiğinde öğenin konumu) **AffectedItems** alanında görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="62ff4-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="62ff4-115">**Clıtinfostring** özelliği, silme işleminin Outlook, Web üzerinde Outlook (önceki adıyla Outlook Web App) veya başka bir cihazdan silinmesi durumunda gösterilir.</span><span class="sxs-lookup"><span data-stu-id="62ff4-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="62ff4-116">Daha fazla bilgi için, [posta kutusu için e-posta iletmeyi kimlerin görebileceğini belirleme](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="62ff4-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="62ff4-117">**Not**: denetim günlüğü özelliğini kullanarak silinmiş öğeleri alamazsınız.</span><span class="sxs-lookup"><span data-stu-id="62ff4-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="62ff4-118">Web üzerinde Outlook 'ta silinmiş iletileri almak için, [Outlook Web App 'te silinmiş öğeleri kurtarma](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="62ff4-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
