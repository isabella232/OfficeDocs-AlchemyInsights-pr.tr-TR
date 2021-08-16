---
title: Intune ile Koşullu Erişim
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069732"
---
# <a name="conditional-access-with-intune"></a>Intune ile Koşullu Erişim

Intune  **ile**  Koşullu Erişimi kullanmak için 3 adım gerekir:

- Cihazın uyumlu **kabul edilene** kadar karşılanmalıdır ayarları tanımlamak için Uyumluluk İlkesi ([Android,](https://docs.microsoft.com/intune/compliance-policy-create-android) [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) oluşturun. Örneğin, bir cihazın uyumlu kabul edilene kadar en az 6 basamaklı bir PIN kodu olmalıdır.
- Korunan **kaynakları ve bu**  kaynaklara erişmek için karşı korunması gereken koşulları tanımlayan bir Koşullu Erişim İlkesi oluşturun.  [Örneğin, bir](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  cihaz şirket e-postalarına erişmek için uyumlu olmalıdır.
- İstediğiniz kullanıcı **gruplarının hem**  **Uyumluluk İlkelerine**  hem de Koşullu Erişim İlkelerine hedef olduğundan emin olun. Bunun için, çalışma sayfalarında belirli kullanıcı grupları Azure Active Directory.

**Yararlı bağlantılar:**

[Cihaz uyumluluğuna genel bakış](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA sorunlarını giderme](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Sorun giderme ilkesi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Uyumlu olmayan cihazlar tarafından E-Exchange(çevrimiçi) erişimini korumak için her iki belge de takip edilecektir:

1. [EAS kullanarak cihazlardan e-posta erişimini koruma](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [E-posta erişimini, e-posta gibi modern kimlik doğrulama istemcilerini kullanarak Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)