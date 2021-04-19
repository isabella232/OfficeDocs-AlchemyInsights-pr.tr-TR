---
title: Aktarım kurallarında DLP kullanma
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827236"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="8b4ce-102">Aktarım kurallarında DLP kullanma</span><span class="sxs-lookup"><span data-stu-id="8b4ce-102">Using DLP in transport rules</span></span>

<span data-ttu-id="8b4ce-103">Veri Kaybı Önleme’yi mevcut aktarımla tümleştirmek için Aktarım kuralı ayarında "**İleti...gizli bilgiler içeriyorsa**" koşulunu kullanın.</span><span class="sxs-lookup"><span data-stu-id="8b4ce-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="8b4ce-104">**Diğer ayrıntılar için bkz:**</span><span class="sxs-lookup"><span data-stu-id="8b4ce-104">**For more details, see:**</span></span>

- <span data-ttu-id="8b4ce-105">Aktarım kurallarındaki tümleşik DLP gizli bilgi türleri: [Gizli Bilgi Kurallarını Tümleştirme](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="8b4ce-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="8b4ce-106">Ayrıca kuralda Test Modunu kullanarak kuralı ilkeyle veya ilke olmadan test edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8b4ce-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="8b4ce-107">Kuralı oluşturduktan sonra test etmek için 30 dakika beklemelisiniz.</span><span class="sxs-lookup"><span data-stu-id="8b4ce-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="8b4ce-108">Bkz. [Posta Akışı/Aktarım kurallarını test etme](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="8b4ce-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="8b4ce-109">**Not**: EAC’de aktarım kurallarıyla yeni bir DLP ilkesi uygulamayı deniyorsanız, bunun yerine [Güvenlik ve Uyumluluk merkezinde DLP İlkeleri](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide)’ni kullanın.</span><span class="sxs-lookup"><span data-stu-id="8b4ce-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
