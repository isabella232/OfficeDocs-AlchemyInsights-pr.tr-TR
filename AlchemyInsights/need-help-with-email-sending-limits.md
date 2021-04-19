---
title: E-posta gönderme sınırları için yardıma mı ihtiyacınız var?
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
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836299"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="6ddaf-102">E-posta gönderme sınırları için yardıma mı ihtiyacınız var?</span><span class="sxs-lookup"><span data-stu-id="6ddaf-102">Need help with email sending limits?</span></span>

<span data-ttu-id="6ddaf-103">Aşağıda, **hizmette zorunlu kılınan tasarıma** göre gönderme sınırları verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="6ddaf-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="6ddaf-104">Bu sınırlar hakkında daha fazla bilgi burada [belgelenmiştir.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)</span><span class="sxs-lookup"><span data-stu-id="6ddaf-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="6ddaf-105">Talep edilmemiş toplu iletilerin teslimini engellememek için, tüm giden ve iç iletilere kullanıcı başına **alıcı oranı sınırları uygulanır.**</span><span class="sxs-lookup"><span data-stu-id="6ddaf-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="6ddaf-106">Tüm SKus'larda, bu sınır günde **10.000 alıcıdır.**</span><span class="sxs-lookup"><span data-stu-id="6ddaf-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="6ddaf-107">Yasal toplu ticari e-posta göndermesi gereken müşteriler (örneğin, müşteri bültenleri) bu hizmetlerde özelleştirilmiş üçüncü taraf sağlayıcıları kullan adresleri kullanır.</span><span class="sxs-lookup"><span data-stu-id="6ddaf-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="6ddaf-108">**Not:** Alıcı oranı sınırına ulaşıldıktan sonra, son 24 saat içinde ileti gönderen alıcıların sayısı sınırın altına inene kadar posta kutusundan ileti gönder kabul edilir.</span><span class="sxs-lookup"><span data-stu-id="6ddaf-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="6ddaf-109">Kullanıcı, bu noktaya kadar ileti gönderemayacak.</span><span class="sxs-lookup"><span data-stu-id="6ddaf-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="6ddaf-110">Tüm **SLU'larda dakikada 30** ileti için ileti hızı sınırı uygulanır.</span><span class="sxs-lookup"><span data-stu-id="6ddaf-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="6ddaf-111">Bu, kullanıcının belirli bir süre içinde Exchange Online hesabından kaç ileti göndere bir olduğunu belirler.</span><span class="sxs-lookup"><span data-stu-id="6ddaf-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="6ddaf-112">Tüm SLU'larda, tek bir e-posta iletisi için **To, Bilgi** ve Gizli alanlarında izin verilen en fazla alıcı sayısı **1000 alıcıdır.**</span><span class="sxs-lookup"><span data-stu-id="6ddaf-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="6ddaf-113">Bu sınırı özelleştirmek için buraya [gidin.](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)</span><span class="sxs-lookup"><span data-stu-id="6ddaf-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
