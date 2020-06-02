---
title: Denetim günlüklerinde IP adresini ve istemciyi belirleme
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508936"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="61647-102">Denetim günlüklerinde IP adresini ve istemciyi belirleme</span><span class="sxs-lookup"><span data-stu-id="61647-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="61647-103">Bir Microsoft 365 kullanıcısı veya yöneticisinin bir etkinliğine karşılık gelen IP adresi Denetim Günlükleri'nde gösterilir.</span><span class="sxs-lookup"><span data-stu-id="61647-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="61647-104">İstemci bilgileri de günlüğe kaydedilir.</span><span class="sxs-lookup"><span data-stu-id="61647-104">The client information is also logged.</span></span> <span data-ttu-id="61647-105">Bu tür bilgileri tanımlamaya ilişkin adımlar şunlardır:</span><span class="sxs-lookup"><span data-stu-id="61647-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="61647-106">[Microsoft 365 Güvenlik & Uyumluluk Merkezi'nde](https://protection.office.com/)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="61647-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="61647-107">**Arama**  >  **Denetimi günlüğü arama** sayfasına gidin.</span><span class="sxs-lookup"><span data-stu-id="61647-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="61647-108">Belirli bir etkinlikle ilgileniyorsanız, **Etkinlikler** listesinden seçin.</span><span class="sxs-lookup"><span data-stu-id="61647-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="61647-109">Değilse, tüm etkinlikler seçili kullanıcı (varsayılan ayar) için döndürülür.</span><span class="sxs-lookup"><span data-stu-id="61647-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="61647-110">**Not**: **Etkinlikler** menüsünde belirli etkinlikler bulunamayabilir; ancak, **tüm etkinliklerin Sonuçlarını Gösterir** seçilirse (varsayılan ayar) bu denetim öğeleri döndürülür.</span><span class="sxs-lookup"><span data-stu-id="61647-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="61647-111">**Kullanıcılar** alanında kullanıcı adını belirtin, etkinlik için uygun tarih aralığını seçin ve ardından **Ara'yı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="61647-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="61647-112">Sonuçlarda, bu etkinliğin IP adresini sonuç bölmesinde görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="61647-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="61647-113">**Ayrıntılar** uçuşundaki ayrıntılı bilgileri görmek için denetim kaydını seçin (örneğin, Müşteri, eylem gerçekleştiren Kullanıcı vb.).</span><span class="sxs-lookup"><span data-stu-id="61647-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="61647-114">Daha fazla bilgi için bkz: [Gizliliği ihlal edilen bir hesaba erişmek için kullanılan bilgisayarın IP adresini bulma.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)</span><span class="sxs-lookup"><span data-stu-id="61647-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
