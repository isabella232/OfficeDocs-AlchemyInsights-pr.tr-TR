---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821467"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Hata kodu 550 5.4.1 Geçiş Erişimi Reddedildi hata kodu için teslim sorunlarını düzeltme

Microsoft ağına girerken [geri dönüşleri önlemek için bir e-posta](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) adresinin geçerli olup olmadığını kontrol etmek bu soruna neden olur. Şunları deneyin:

1. Sorunun bir etki alanının tamamına mı yoksa tek bir e-posta adresine mi özgü olduğunu belirleme:
    - Tüm etki alanı: Bazen etki alanının eşitlenmesi gerekir; etki [alanını İç olarak ayarlamayı deneyin ve sonra Yetkili ayarına geri dönebilirsiniz.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Tek e-posta adresi: Bazen adresin eşitlenmesi gerekir; smtp ara sunucu adresini değiştirmek ve sonra yeniden değiştirmek yardımcı olabilir.
2. Sorunun bir gruba mı yoksa ortak klasöre mi özel olduğunu belirler. Bazı nesne türlerinde, nesnelerin Azure Active Directory'de el ile oluşturulmuş olması gerekebilir.

Daha fazla yardım gerekirse, lütfen bir destek bileti açın ve size daha iyi yardımcı olmak için sorunun kapsamını (gönderirken hangi tür nesne dahil) belirtin.