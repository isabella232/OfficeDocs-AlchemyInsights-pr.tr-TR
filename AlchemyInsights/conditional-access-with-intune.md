---
title: Intune ile Koşullu Erişim
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931456"
---
# <a name="conditional-access-with-intune"></a>Intune ile Koşullu Erişim

**Koşullu Erişimi** Intune ile kullanmak 3 adım gerektirir:

- Aygıt **uyumlu** kabul edilmeden önce karşılanması gereken ayarları tanımlamak için bir Uyumluluk Politikası[(Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)oluşturun. Örneğin, bir aygıtın uyumlu kabul edilmeden önce en az 6 basamaklı bir iğneye sahip olması gerekir.
- Hangi kaynakların korunduğunu ve bu kaynaklara erişmek için hangi koşulların karşılanması gerektiğini tanımlayan **koşullu erişim ilkesi** oluşturun.  [Örneğin,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) bir aygıtın şirket e-postasına erişmeden önce uyumlu olması gerekir.
- Hem **Uyumluluk İlkeleri'nin** hem de **Koşullu Erişim İlkelerinin** istenilen kullanıcı gruplarına hedef olduğundan emin olun. Bu, Azure Etkin Dizini'nde belirli kullanıcı grupları oluşturulmasını gerektirebilir.

**Yararlı bağlantılar:**

[Cihaz uyumluluğuna genel bakış](https://docs.microsoft.com/intune/device-compliance-get-started)

[SORUN Giderme CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Sorun giderme ilkesi](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

E-postayı (Çevrimiçi Exchange) uyumlu olmayan aygıtların erişiminden korumak için her iki belgeye de uyulmalıdır:

1. [EAS kullanan cihazlardan e-posta erişimini koruma](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Outlook gibi modern kimlik doğrulama istemcilerini kullanan aygıtlardan e-posta erişimini koruma](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)