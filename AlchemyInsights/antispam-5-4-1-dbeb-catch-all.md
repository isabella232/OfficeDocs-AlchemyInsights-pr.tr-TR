---
title: AntiSpam 5.4.1 VSEÇŞB yakala-tümü
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717381"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Hata kodu 550 5.4.1 geçiş erişimi reddedildi için teslim sorunlarını düzeltme

Bu sorun, Microsoft ağını girerken geri [sıçramasını önleyen bir e-posta adresinin geçerli olup olmadığını denetlemek için](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) görülür. Aşağıdakileri deneyin:

1. Sorunun tüm etki alanına mı yoksa tek bir e-posta adresine mi özgü olduğunu belirleme:
    - Tüm etki alanı: bazen etki alanının eşitlenmesi gereklidir; [etki alanını iç öğesine ayarlamayı ve ardından yetkilendirmeli 'a geri dönün](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Tek e-posta adresi: bazen adresin eşitlenmesi gereklidir; SMTP proxy adresini değiştirip geri değiştirmek yardım edebilir.
2. Sorunun bir gruba veya ortak klasöre özgü olup olmadığını belirleme. Bazı nesne türlerinde, nesnelerin Azure Active Directory 'de el ile oluşturulması gerekebilir.

Ek yardıma ihtiyacınız varsa, lütfen bir destek bileti açın ve sorunun kapsamını (göndermekte olduğunuz nesnenin türü de dahil olmak üzere) belirtin, böylece daha iyi yardımcı olabiliriz.