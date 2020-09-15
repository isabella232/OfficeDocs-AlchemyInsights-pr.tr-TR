---
title: Dış grupları devre dışı bırakma
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704148"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="67f07-102">Dış grupları devre dışı bırakma</span><span class="sxs-lookup"><span data-stu-id="67f07-102">How to disable External Groups</span></span>

<span data-ttu-id="67f07-103">Yammer dış mesajlaşma, şirket bilgilerinin paylaşılmasını önleyen bir dizi önleyici denetim olan Exchange aktarma kuralları 'nı (ETRs) uygular.</span><span class="sxs-lookup"><span data-stu-id="67f07-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="67f07-104">Kullanıcıların dış gruplar oluşturmasını engellemek için, bir Exchange aktarma kuralı (ETR) yapılandırmanız ve ardından Yammer 'ı, dış iletileri engellemek üzere Exchange Aktarım kuralını kullanacak şekilde yapılandırmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="67f07-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="67f07-105">Exchange Online Yönetim merkezinde bir kural oluşturduktan sonra, ETR 'i Yammer 'da uygulanacak şekilde ayarlamak için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="67f07-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="67f07-106">Yammer 'da doğrulanmış yönetici olarak oturum açın ve **Yammer Yönetim merkezinde**C **içeriği ve güvenlik \> güvenliği ayarları** 'na gidin.</span><span class="sxs-lookup"><span data-stu-id="67f07-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="67f07-107">**Dış mesajlaşma**'nın altında, **Yammer 'Da Exchange Online Exchange aktarma kurallarınızı (ETRs) zorla** 'yı seçin.</span><span class="sxs-lookup"><span data-stu-id="67f07-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="67f07-108">**Kaydet**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="67f07-108">Choose **Save**.</span></span>

<span data-ttu-id="67f07-109">Daha fazla bilgi için bkz [.](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)</span><span class="sxs-lookup"><span data-stu-id="67f07-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  