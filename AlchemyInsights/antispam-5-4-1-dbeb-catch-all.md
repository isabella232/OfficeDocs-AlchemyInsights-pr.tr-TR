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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707931"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Hata kodu 550 5.4.1 Röle Erişimi Reddedildi için teslim sorunlarını düzeltme

Bu sorun, Microsoft ağına girerken [geri dönüşleri önlemek için bir e-posta adresinin geçerli olup olmadığını kontrol](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ederken oluşur. Aşağıdakileri deneyin:

1. Sorunun tüm etki alanına mı yoksa tek bir e-posta adresine mi özgü olduğunu belirleyin:
    - Tüm etki alanı: Bazen etki alanının eşitlemesi gerekir; [etki alanını İçe ayarlamayı deneyin ve ardından Yetkili'ye geri dönmeyi](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)deneyin.
    - Tek e-posta adresi: Bazen adresin senkronize edilmesi gerekir; smtp proxy adresini değiştirmek ve sonra geri değiştirme yardımcı olabilir.
2. Sorunun bir gruba mı yoksa ortak klasöre mi özgü olduğunu belirleyin. Bazı nesne türleri için nesnelerin Azure Etkin Dizini'nde el ile oluşturulması gerekebilir.

Ek yardıma ihtiyacınız varsa, size daha iyi yardımcı olmamız için lütfen bir destek bileti açın ve sorunun kapsamını (gönderdiğiniz nesnenin türü dahil) belirtin.