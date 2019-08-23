---
title: 1332 - OWA gelen kutusu kuralları bir posta kutusu için yürütülen değil
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 901237d4dc7b99695097142c61a4bfef7c09750d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36555793"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="cb8fa-102">Gelen kutusu kuralı beklendiği gibi çalışmıyor</span><span class="sxs-lookup"><span data-stu-id="cb8fa-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="cb8fa-103">Web'de Outlook'taki aşağıdaki ayarları doğrulayın:</span><span class="sxs-lookup"><span data-stu-id="cb8fa-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="cb8fa-104">Bir ileti, iletilen veya yanıtlanan dayanarak otomatik olarak gelen kutusu kuralları üzerinde yalnızca bir kez yeniden yönlendirilebilir.</span><span class="sxs-lookup"><span data-stu-id="cb8fa-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="cb8fa-105">Bir yeniden yönlendirme kuralı (bir gelen kutusu kuralı veya posta akışı kuralı, bir aktarım kuralı olarak da bilinir) en çok on iletme alıcıların iletiye ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cb8fa-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="cb8fa-106">[Günlük, taşıma ve gelen kutusu kuralı sınırlarını](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="cb8fa-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="cb8fa-107">Gelen Kutusu kuralları diğer günlük kaydı posta kutusunun üzerinde çalışmaz.</span><span class="sxs-lookup"><span data-stu-id="cb8fa-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="cb8fa-108">[Diğer günlük kaydı posta kutusu](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)posta kutusu diğer günlük kaydı hakkında daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="cb8fa-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="cb8fa-109">Bu sorunları gidermek için bkz: [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="cb8fa-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="cb8fa-110">Yukarıdaki sorunlar uygulamazsanız, Microsoft Support sorunu üst düzeye iletmeden önce gelen kutusu kuralı Tanılama raporunu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="cb8fa-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="cb8fa-111">Web'de Outlook'taki posta kutusunu açın ve'ı tıklatın</span><span class="sxs-lookup"><span data-stu-id="cb8fa-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="cb8fa-112">**Ayarları** > **tüm Outlook ayarları görüntülemek** > **posta** > **kurallar**.</span><span class="sxs-lookup"><span data-stu-id="cb8fa-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="cb8fa-113">Sayfanın alt kısmında, **kurallarınızın bir tanılama raporu oluşturmak için burayı tıklatın çalışıyorsanız değil'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="cb8fa-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
