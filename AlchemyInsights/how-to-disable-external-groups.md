---
title: Dış Gruplar nasıl devre dışı edilir?
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36739513"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="47dc0-102">Dış Gruplar nasıl devre dışı edilir?</span><span class="sxs-lookup"><span data-stu-id="47dc0-102">How to disable External Groups</span></span>

<span data-ttu-id="47dc0-103">Yammer harici mesajlaşma, şirket bilgilerinin paylaşılmasını önlemek için bir dizi proaktif denetim olan Exchange Transport Rules (ETR) uygular.</span><span class="sxs-lookup"><span data-stu-id="47dc0-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="47dc0-104">Kullanıcıların dış gruplar oluşturmasını kısıtlamak için, bir Exchange aktarım kuralını (ETR) yapılandırmanız ve ardından Yammer'ı dış iletileri engellemek için Exchange Aktarım kuralını kullanacak şekilde yapılandırmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="47dc0-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="47dc0-105">Exchange Online yönetici merkezinde bir kural oluşturduktan sonra, ETR'yi Yammer'da uygulanacak şekilde ayarlamak için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="47dc0-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="47dc0-106">Doğrulanmış bir yönetici olarak Yammer'da oturum açın ve **Yammer yönetici merkezinde**C **İçerik ve \> Güvenlik Ayarları'na gidin.**</span><span class="sxs-lookup"><span data-stu-id="47dc0-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="47dc0-107">**Harici İleti altında,** **Yammer'daki Exchange Online Exchange Aktarım Kurallarınızı (ETR) uygulayın'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="47dc0-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="47dc0-108">**Kaydet**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="47dc0-108">Choose **Save**.</span></span>

<span data-ttu-id="47dc0-109">Daha fazla bilgi için, [bir Yammer ağında harici iletileri devre dışı bırakın.](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)</span><span class="sxs-lookup"><span data-stu-id="47dc0-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  