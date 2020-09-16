---
title: Gereksiz e-posta klasörüne giden e-posta
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
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769203"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="3d0dc-102">Gereksiz e-posta klasörüne giden e-posta</span><span class="sxs-lookup"><span data-stu-id="3d0dc-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="3d0dc-103">Gereksiz olarak işaretlenmiş iletileri görüyorsanız aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="3d0dc-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="3d0dc-104">Şimdiye kadar yapmadıysanız, [giden istenmeyen ilke bildirimlerini yapılandırmayı](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)düşünebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="3d0dc-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="3d0dc-105">[İleti izleme](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) 'yi kullanarak, giden iletide ek ayrıntılara sahip istenmeyen olay değerinin **gereksiz** olduğunu görebilirsiniz: **yüksek riskli teslim havuzu kullanın**.</span><span class="sxs-lookup"><span data-stu-id="3d0dc-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="3d0dc-106">Bu iletiler için, ileti içeriğini denetleyerek istenmeyen posta olarak ne olabileceğini görün.</span><span class="sxs-lookup"><span data-stu-id="3d0dc-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="3d0dc-107">Örneğin, imzalar bazen birçok kullanıcı için sorunlara neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="3d0dc-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="3d0dc-108">Gereksiz olarak işaretlenmiş uygun giden ileti örneklerine sahipseniz, bir destek bileti açın ve destek aracısından iletilerinizin istenmeyen posta anallerimize yanlış pozitif olarak göndermesini isteyin.</span><span class="sxs-lookup"><span data-stu-id="3d0dc-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="3d0dc-109">Tüm ileti üstbilgilerini içeren örnek iletiler vermeye hazırlıklı olun.</span><span class="sxs-lookup"><span data-stu-id="3d0dc-109">Be prepared to provide sample messages that include all message headers.</span></span>
