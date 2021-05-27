---
title: Saldırı yüzeyini azaltma kuralları
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676570"
---
# <a name="attack-surface-reduction-rules"></a>Saldırı yüzeyini azaltma kuralları

Dosya veya klasörlerin dışlamaları saldırı yüzeyini azaltma kuralları tarafından sağlanan korumayı ciddi ölçüde azaltır. Kural tarafından engellenmiş olan dosyaların çalışmasına izin verilir ve hiçbir rapor veya olay kaydedilmiyor. Dışlama, dışlamalara izin olan tüm kurallara uygulanır.

ASR dışlamaları, dışlamalarda olduğu gibi Microsoft Defender Virüsten Koruma kullanır. Ayrıntılar için bkz. [Taramalarda dışlamaları yapılandırma Microsoft Defender Virüsten Koruma doğrulama.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) Sorunlardan kaçınmak için, [dışlamaları tanımlarken kaçınılması gereken yaygın hataları gözden geçirin.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

Tüm ASR kuralları dışlamaları desteklemez. Kuralınız dışlamaları destekleyip desteklemedi bunu doğrulamak için Saldırı yüzeyini azaltma [kuralları tablosuna bakın.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

## <a name="attack-surface-reduction-rules"></a>Saldırı yüzeyini azaltma kuralları

Organizasyon saldırı yüzeyiniz, bir saldırganın kuruluş cihazlarını veya ağlarını tehlikeye atabilmesi için güvenlik ödünleri olan tüm yerleri içerir. Saldırı yüzeyinizi azaltmak, kuruluş cihazlarını ve ağın korunması anlamına gelir; bu da saldırı gerçekleştirmek için daha az yol bırakır. Uç nokta için Microsoft Defender'da saldırı yüzeyini azaltma kurallarını yapılandırmanıza yardımcı olabilir.

Daha fazla bilgi için bkz.:

- [ASR kuralı GUID'lerini adla eşleme](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- ASR kuralları gereksinimleri:
    - [Windows 10 Pro, sürüm 1709 veya sonrası](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, sürüm 1709 veya sonrası](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Sunucu, sürüm 1803 (Yarı Yıllık Kanal) veya sonraki sürümler](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Uygulanacak doğru dışlamayı belirleme

1. Microsoft-Windows-Windows Defender/Operational günlüğünde eventID 1121 veya 1122'i bakın.

1. Engelleme senaryosunu ve bağlamı değerlendirin ve bu senaryonun engellemesini kaldırmanız gerektiğini onaylayın.

1. Olay ayrıntılarında Yol değerini okuyun; bu, dışlamayı tanımlayan değerdir.
    - Dışlama mümkün olduğunca katı hale geldi.
    - Gerektiğinde bir joker karakter uygulayabilirsiniz (örneğin, Kullanıcı değişkeninin yerini değiştirin).

1. Dışlamayı dağıtım ihtiyaçlarına göre uygulayabilirsiniz. Ayrıntılı bilgi için Saldırı [yüzeyini azaltma kurallarını özelleştirme .](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)

## <a name="exclusion-is-not-honored"></a>Dışlamalara devam etmek mümkün değil

1. Kuralın dışlamalarını destekle ilgili olup olmadığını belirler. Ayrıntılı bilgi için Saldırı [yüzeyini azaltma kuralları 'ne bakın.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

1. Uygulanan dışlamaları gözden geçirme ve yazım hataları veya yanlış yapılan joker karakterlerle ilgili olay verileriyle doğrulama. Daha fazla bilgi için [bkz. Desteklenen dışlama türleri](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. kuralın etkisi çok yüksekse, daha fazla doğrulama gerçekleştirmek için kuralı (geri) Denetim moduna taşımayı göz önünde bulundurabilirsiniz. Ayrıntılar için bkz. [Uç nokta özellikleri için Microsoft Defender'ın denetim modunda nasıl çalışacı olduğunu test edin.](/microsoft-365/security/defender-endpoint/audit-windows-defender)

1. Bu komutu kullanarak destek olaylarını açmak için destek verilerini toplayın:
    
   ** MDEClientAnalyzer.cmd -v**

    Daha fazla bilgi için [bkz. Uç Noktalar için Microsoft Defender'a makine ekleme ile ilgili sorunlar.](issues-with-onboarding-machines.md)
