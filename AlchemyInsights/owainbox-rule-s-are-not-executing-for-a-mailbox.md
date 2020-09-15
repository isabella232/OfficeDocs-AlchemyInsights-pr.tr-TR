---
title: 1332 OWA-posta kutusu kuralları için gelen kutusu kuralları yürütülmüyor
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
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721611"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Gelen kutusu kuralı beklendiği gibi çalışmıyor

Web üzerinde Outlook 'ta aşağıdaki ayarları doğrulayın:

- İleti otomatik olarak, gelen kutusu kurallarına göre otomatik olarak yönlendirilebilir, iletilebilir veya yanıtlanır. Yeniden yönlendirme kuralı (aktarım kuralı olarak da bilinen bir gelen kutusu kuralı veya posta akış kuralı), bir iletiye en fazla on sayıda iletme alıcısı ekleyebilir. Daha fazla bilgi için, [bkz.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- Gelen kutusu kuralları alternatif günlük kaydı posta kutusunda çalışmaz. Alternatif günlük kaydı posta kutusu hakkında daha fazla bilgi için [bkz.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

Bu sorunları düzeltmek için, [KB 2829319](https://support.microsoft.com/kb/2829319)bakın.

Önceki sorunlar geçerli değilse, sorunu Microsoft desteğine göndermeden önce gelen kutusu kuralı tanı raporunu çalıştırabilirsiniz:

1. Web üzerinde Outlook posta kutusunu açın ve <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Ayarları**  >  **Tüm Outlook ayarlarını görüntüleme**  >  **Posta**  >  **Kuralları**.

2. Sayfanın en altında, **kurallarınız çalışmıyorsa, bir tanılama raporu oluşturmak için buraya tıklayın**.
