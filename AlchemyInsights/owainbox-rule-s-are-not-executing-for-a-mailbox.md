---
title: 1332 OWA - Gelen Kutusu kuralı(lar) posta kutusu için yürütülmez
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576580"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Gelen Kutusu kuralı beklendiği gibi çalışmıyor

Web'de Outlook'ta aşağıdaki ayarları doğrulayın:

- İleti, Gelen Kutusu kurallarına göre yalnızca bir kez yeniden yönlendirilebilir, iletilebilir veya otomatik olarak yanıtlanabilir. Yeniden yönlendirme kuralı (gelen kutusu kuralı veya ileti akışı kuralı olarak da bilinir) iletiye en fazla on iletme alıcısı ekleyebilir. Daha fazla bilgi için [Bkz. Günlük, Aktarım ve Gelen Kutusu kural sınırları.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- Gelen kutusu kuralları alternatif günlük posta kutusunda çalışmaz. Alternatif günlük posta kutusu hakkında daha fazla bilgi için [Alternatif günlük posta kutusuna](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)bakın.

Bu sorunları gidermek için [KB 2829319'a](https://support.microsoft.com/kb/2829319)bakın.

Önceki sorunlar geçerli değilse, sorunu Microsoft Desteği'ne yükseltmeden önce Gelen Kutusu kuralı tanılama raporunu çalıştırın:

1. Web'de Outlook'ta posta kutusunu açın ve <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Ayarlar**  >  **Tüm Outlook Ayarlarını**  >  Görüntüle **Posta**  >  **Kurallar.**

2. Sayfanın alt kısmında, **kurallarınız çalışmıyorsa bir tanılama raporu oluşturmak için burayı tıklatın.**
