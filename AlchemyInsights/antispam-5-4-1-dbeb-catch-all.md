---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672453"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Hata kodu 550 5.4.1 Röle Erişimi Reddedildi için teslim sorunlarını düzeltme

Bu sorun, Office 365 ağına girerken [geri dönüşleri önlemek için bir e-posta adresinin geçerli olup olmadığını kontrol](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ederken oluşur. Aşağıdakileri deneyin:

1. Sorunun tüm etki alanına mı yoksa tek bir e-posta adresine mi özgü olduğunu belirleyin:
    - Tüm etki alanı: Bazen etki alanının eşitlemesi gerekir; [etki alanını İçe ayarlamayı deneyin ve ardından Yetkili'ye geri dönmeyi](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)deneyin.
    - Tek e-posta adresi: Bazen adresin senkronize edilmesi gerekir; smtp proxy adresini değiştirmek ve sonra geri değiştirme yardımcı olabilir.
2. Sorunun bir gruba mı yoksa ortak klasöre mi özgü olduğunu belirleyin. Bazı nesne türleri için nesnelerin Azure Etkin Dizini'nde el ile oluşturulması gerekebilir.

Ek yardıma ihtiyacınız varsa, size daha iyi yardımcı olmamız için lütfen bir destek bileti açın ve sorunun kapsamını (gönderdiğiniz nesnenin türünü dahil) belirtin.