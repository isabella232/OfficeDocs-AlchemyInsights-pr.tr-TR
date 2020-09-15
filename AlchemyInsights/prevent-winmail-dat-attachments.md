---
title: 2589 kuruluşunuzdaki e-posta iletilerinde Winmail. dat eklerinin engellenmesine yardımcı olun
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: f67c4146af419a590651c8e0673fd59fabd7eae7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47693755"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="adfe3-102">Kuruluşunuzdan gelen e-posta iletilerinde Winmail. dat eklerinin engellenmesine yardımcı olun</span><span class="sxs-lookup"><span data-stu-id="adfe3-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="adfe3-103">Yönetici olarak aşağıdaki adımları deneyin:</span><span class="sxs-lookup"><span data-stu-id="adfe3-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="adfe3-104">[Exchange Yönetim merkezini](https://outlook.office365.com/ecp/)açın.</span><span class="sxs-lookup"><span data-stu-id="adfe3-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>

2. <span data-ttu-id="adfe3-105">**Posta akışı**  >  **uzak etki alanlarına**gidin.</span><span class="sxs-lookup"><span data-stu-id="adfe3-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="adfe3-106">**Varsayılan**adlı varsayılan uzak etki alanını seçin ve **Düzenle**'yi tıklatın.</span><span class="sxs-lookup"><span data-stu-id="adfe3-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="adfe3-107">**Zengin metin biçimi kullan** bölümünde **hiçbir zaman**öğesini seçin.</span><span class="sxs-lookup"><span data-stu-id="adfe3-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="adfe3-108">Daha fazla bilgi için bkz [.](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format)</span><span class="sxs-lookup"><span data-stu-id="adfe3-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
