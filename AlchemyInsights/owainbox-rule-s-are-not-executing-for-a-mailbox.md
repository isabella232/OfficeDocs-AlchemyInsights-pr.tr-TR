---
title: 1332 OWA - Gelen Kutusu kuralları posta kutusu için yürütülemz
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040922"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Gelen Kutusu kuralı beklendiği gibi çalışmıyor

E-postada aşağıdaki ayarları Web üzerinde Outlook:

- Bir ileti yalnızca bir kez Gelen Kutusu kurallarına göre yeniden yönlendirilmesi, iletilmesi veya otomatik olarak yanıtilmesine neden olabilir. Yeniden yönlendirme kuralı (Gelen Kutusu kuralı veya posta akışı kuralı, aktarım kuralı olarak da bilinir) bir iletiye en çok on iletme alıcısı ekleyebilir. Daha fazla bilgi için [bkz. Günlük, Aktarım ve Gelen Kutusu kural sınırları.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- Gelen kutusu kuralları diğer günlük günlüğü posta kutusunda çalışmıyor. Alternatif günlük günlüğü posta kutusu hakkında daha fazla bilgi için [bkz. Alternatif günlük günlüğü posta kutusu.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

Bu sorunları çözmek için bkz. [KB 2829319.](https://support.microsoft.com/kb/2829319)

Önceki sorunlar geçerli olmazsa, sorunu Microsoft Desteği'ne yükseltmeden önce Gelen Kutusu kuralı tanılama raporunu çalıştırın:

1. Posta kutusunu Aynı Web üzerinde Outlook açın ve <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Ayarlar**  >  **Tüm e-Outlook Ayarlar**  >  **Posta**  >  **Kurallar**.

2. Sayfanın en altında, Kurallarınız çalışmıyorsa buraya **tıklayın ve tanılama raporu oluşturmak için tıklayın.**
