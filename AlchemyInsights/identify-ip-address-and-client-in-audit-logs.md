---
title: Denetim günlüklerinde IP adresini ve istemciyi belirleme
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668330"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="1f1ea-102">Denetim günlüklerinde IP adresini ve istemciyi belirleme</span><span class="sxs-lookup"><span data-stu-id="1f1ea-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="1f1ea-103">Microsoft 365 kullanıcısına veya yöneticisine karşılık gelen IP adresi denetim günlüklerinde gösterilir.</span><span class="sxs-lookup"><span data-stu-id="1f1ea-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="1f1ea-104">İstemci bilgileri de günlüğe kaydedilir.</span><span class="sxs-lookup"><span data-stu-id="1f1ea-104">The client information is also logged.</span></span> <span data-ttu-id="1f1ea-105">Bu tür bilgileri tanımlama adımları şunlardır</span><span class="sxs-lookup"><span data-stu-id="1f1ea-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="1f1ea-106">[Microsoft 365 güvenlik & Uyumluluk Merkezi](https://protection.office.com/)'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="1f1ea-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="1f1ea-107">**Search**  >  **Denetim günlüğü aramasını** ara sayfasına gidin.</span><span class="sxs-lookup"><span data-stu-id="1f1ea-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="1f1ea-108">Belirli bir etkinlikle ilgileniyorsa, **etkinlik** listesinden bunu seçin.</span><span class="sxs-lookup"><span data-stu-id="1f1ea-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="1f1ea-109">Değilse, tüm etkinlikler seçilen kullanıcı için geri döndürülecek (varsayılan ayar).</span><span class="sxs-lookup"><span data-stu-id="1f1ea-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="1f1ea-110">**Not**: **Etkinlikler** menüsünde bazı etkinlikler kullanılamayabilir; Ancak, **tüm etkinlikler Için sonuçları göster** seçildiğinde bu denetim öğeleri döndürülür (varsayılan ayar).</span><span class="sxs-lookup"><span data-stu-id="1f1ea-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="1f1ea-111">**Kullanıcı alanında Kullanıcı** adını belirtin, etkinlik için uygun tarih aralığını seçin ve **Ara**'ya tıklayın.</span><span class="sxs-lookup"><span data-stu-id="1f1ea-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="1f1ea-112">Sonuçlarda, bu etkinliğin IP adresini sonuçlar bölmesinde görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1f1ea-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="1f1ea-113">**Ayrıntılar** açılır listesinde ayrıntılı bilgileri görmek için denetim kaydını seçin (örneğin, müşteri, eylemi gerçekleştiren kullanıcı vb.).</span><span class="sxs-lookup"><span data-stu-id="1f1ea-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="1f1ea-114">Daha fazla bilgi için, [güvenliği aşılmış bir hesaba erişmek için kullanılan BILGISAYARıN IP adresini bulma](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="1f1ea-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
