---
title: Dış grupları devre dışı bırakma
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399683"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="2c4cb-102">Dış grupları devre dışı bırakma</span><span class="sxs-lookup"><span data-stu-id="2c4cb-102">How to disable External Groups</span></span>

<span data-ttu-id="2c4cb-103">Yammer dış ileti Exchange Aktarım kuralı (ETRs), şirket bilgi paylaşılmasını önlemek için önceden önlem almaya yönelik denetimler kümesi uygular.</span><span class="sxs-lookup"><span data-stu-id="2c4cb-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="2c4cb-104">Kullanıcılar dış grupları oluşturmasını kısıtlamak için Exchange Aktarım kuralı (ETR) yapılandırmak ve sonra Yammer dış iletileri engellemek için Exchange aktarımı kuralı kullanacak şekilde yapılandırmak gerekir.</span><span class="sxs-lookup"><span data-stu-id="2c4cb-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="2c4cb-105">Çevrimiçi Exchange Yönetim Merkezi'nde bir kural oluşturduktan sonra Yammer'da uygulamak için ETR ayarlamak için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="2c4cb-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="2c4cb-106">C sitesine gidin, oturum açmak için Yammer olarak doğrulanan yönetim ve **Yönetim Merkezi Yammer** **önderilen ve güvenlik \> güvenlik ayarlarını.**</span><span class="sxs-lookup"><span data-stu-id="2c4cb-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="2c4cb-107">**Dış ileti**altında seçin **Exchange çevrimiçi Exchange Aktarım kuralları (ETRs) zorla Yammer'da.**</span><span class="sxs-lookup"><span data-stu-id="2c4cb-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="2c4cb-108">**Kaydet**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="2c4cb-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="2c4cb-109">Daha fazla bilgi için bkz: [dış Exchange aktarımı kurallarla Yammer ağında ileti denetimi](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="2c4cb-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

