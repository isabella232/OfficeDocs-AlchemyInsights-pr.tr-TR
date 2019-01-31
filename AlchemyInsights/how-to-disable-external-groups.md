---
title: Dış grupları devre dışı bırakma
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 09d8b134a4e99912301aa92c2e989fec9dd30a7b
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656407"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="2028e-102">Dış grupları devre dışı bırakma</span><span class="sxs-lookup"><span data-stu-id="2028e-102">How to disable External Groups</span></span>

<span data-ttu-id="2028e-p101">Yammer dış ileti Exchange Aktarım kuralı (ETRs), şirket bilgi paylaşılmasını önlemek için önceden önlem almaya yönelik denetimler kümesi uygular. Kullanıcılar dış grupları oluşturmasını kısıtlamak için Exchange Aktarım kuralı (ETR) yapılandırmak ve sonra Yammer dış iletileri engellemek için Exchange aktarımı kuralı kullanacak şekilde yapılandırmak gerekir.</span><span class="sxs-lookup"><span data-stu-id="2028e-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="2028e-105">Çevrimiçi Exchange Yönetim Merkezi'nde bir kural oluşturduktan sonra Yammer'da uygulamak için ETR ayarlamak için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="2028e-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="2028e-106">C sitesine gidin, oturum açmak için Yammer olarak doğrulanan yönetim ve **Yönetim Merkezi Yammer** **önderilen ve güvenlik \> güvenlik ayarlarını.**</span><span class="sxs-lookup"><span data-stu-id="2028e-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="2028e-107">**Dış ileti**altında seçin **Exchange çevrimiçi Exchange Aktarım kuralları (ETRs) zorla Yammer'da.**</span><span class="sxs-lookup"><span data-stu-id="2028e-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="2028e-108">**Kaydet**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="2028e-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="2028e-109">Daha fazla bilgi için bkz: [dış Exchange aktarımı kurallarla Yammer ağında ileti denetimi](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="2028e-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

