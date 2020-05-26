---
title: E-posta gönderme sınırları konusunda yardıma mı ihtiyacınız var?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358361"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="dfafa-102">E-posta gönderme sınırları konusunda yardıma mı ihtiyacınız var?</span><span class="sxs-lookup"><span data-stu-id="dfafa-102">Need help with email sending limits?</span></span>

<span data-ttu-id="dfafa-103">Aşağıda, hizmette uygulanan **yan tasarım gönderme sınırları** verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="dfafa-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="dfafa-104">Bu sınırlar hakkında daha fazla bilgi [burada](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)belgelenmiştir.</span><span class="sxs-lookup"><span data-stu-id="dfafa-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="dfafa-105">İstenmeyen toplu iletilerin teslimini engellemek için, kullanıcı başına **alıcı oranı sınırları tüm giden ve dahili iletilere**uygularız.</span><span class="sxs-lookup"><span data-stu-id="dfafa-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="dfafa-106">Tüm SUS'larda bu sınır **günde 10.000 alıcıdır.**</span><span class="sxs-lookup"><span data-stu-id="dfafa-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="dfafa-107">Yasal toplu ticari e-posta (örneğin, müşteri bültenleri) göndermesi gereken müşteriler, bu hizmetlerde uzmanlaşmış üçüncü taraf sağlayıcıları kullanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="dfafa-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="dfafa-108">**Not**: Alıcı oranı sınırına ulaşıldıktan sonra, son 24 saat içinde ileti gönderilen alıcı sayısı sınırın altına düşene kadar iletiler posta kutusundan gönderilemez.</span><span class="sxs-lookup"><span data-stu-id="dfafa-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="dfafa-109">Kullanıcı bu noktaya kadar ileti gönderemez.</span><span class="sxs-lookup"><span data-stu-id="dfafa-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="dfafa-110">Tüm SK'lerde **dakikada 30 ileti** ileti hızı sınırı uygulanır.</span><span class="sxs-lookup"><span data-stu-id="dfafa-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="dfafa-111">Bu, bir kullanıcının belirli bir süre içinde Exchange Online hesabından kaç ileti gönderebileceğini belirler.</span><span class="sxs-lookup"><span data-stu-id="dfafa-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="dfafa-112">Tüm SK'larda tek bir e-posta iletisi için **To, Cc ve Bcc** alanlarında izin verilen maksimum alıcı sayısı **1000'dir.**</span><span class="sxs-lookup"><span data-stu-id="dfafa-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="dfafa-113">Bu sınırı özelleştirmek için [buraya](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)gidin.</span><span class="sxs-lookup"><span data-stu-id="dfafa-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
