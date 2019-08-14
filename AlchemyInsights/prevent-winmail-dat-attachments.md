---
title: 2589, kuruluşunuzdan e-posta iletilerine Winmail.dat ekleri engellemek
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: 41ab3f22499994cda5883834ff54e5767c69265b
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391595"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="5ddb7-102">E-posta iletilerine Winmail.dat ekleri, kuruluşunuzdan engellemek</span><span class="sxs-lookup"><span data-stu-id="5ddb7-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="5ddb7-103">Bir yönetici olarak aşağıdaki adımları deneyin:</span><span class="sxs-lookup"><span data-stu-id="5ddb7-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="5ddb7-104">[Exchange Yönetim Merkezi'ni](https://outlook.office365.com/ecp/)açın.</span><span class="sxs-lookup"><span data-stu-id="5ddb7-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>

2. <span data-ttu-id="5ddb7-105">**Posta akışı**Git > **Uzak etki alanları**.</span><span class="sxs-lookup"><span data-stu-id="5ddb7-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="5ddb7-106">**Varsayılan**adlı varsayılan uzak etki alanını seçin ve sonra **Düzenle**' yi tıklatın.</span><span class="sxs-lookup"><span data-stu-id="5ddb7-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="5ddb7-107">**Kullanım zengin metin biçimli** bölümünde, **hiçbir zaman**seçeneğini seçin.</span><span class="sxs-lookup"><span data-stu-id="5ddb7-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="5ddb7-108">Daha fazla bilgi için bkz: [Uzak etki alanlarına ileti biçimini belirtin](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span><span class="sxs-lookup"><span data-stu-id="5ddb7-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
