---
title: Önemsiz E-posta klasörüne giden e-posta
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 2350586e95f316061ff855d152e86db0547eb209
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761188"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="5700f-102">Önemsiz E-posta klasörüne giden e-posta</span><span class="sxs-lookup"><span data-stu-id="5700f-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="5700f-103">Giden iletilerin Önemsiz olarak işaretlendiğini görüyorsanız, aşağıdaki adımları yapın:</span><span class="sxs-lookup"><span data-stu-id="5700f-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="5700f-104">Henüz yapmadıysanız, giden [spam ilke bildirimlerini yapılandırmayı](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy)düşünün.</span><span class="sxs-lookup"><span data-stu-id="5700f-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="5700f-105">Giden iletinin ek **ayrıntıyla** birlikte spam olay değerine sahip olup olmadığını görmek için [ileti izlemesini](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) **kullanın: Yüksek riskli teslim havuzunu kullanın.**</span><span class="sxs-lookup"><span data-stu-id="5700f-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="5700f-106">Bu iletiler için, spam olarak kabul edilenene ne olduğunu görmek için ileti içeriğini denetleyin.</span><span class="sxs-lookup"><span data-stu-id="5700f-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="5700f-107">Örneğin, imzalar bazen birçok kullanıcı için sorunlara neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="5700f-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="5700f-108">Önemsiz olarak işaretlenmiş birden çok yasal giden ileti örneğiniz varsa, bir destek bileti açın ve destek temsilcisinden iletilerinizi spam analistlerimize yanlış pozitif olarak göndermesini isteyin.</span><span class="sxs-lookup"><span data-stu-id="5700f-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="5700f-109">Tüm ileti üstbilgilerini içeren örnek iletiler sağlamaya hazır olun.</span><span class="sxs-lookup"><span data-stu-id="5700f-109">Be prepared to provide sample messages that include all message headers.</span></span>
