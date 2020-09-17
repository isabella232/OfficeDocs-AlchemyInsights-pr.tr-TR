---
title: Intune ile koşullu erişim
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807679"
---
# <a name="conditional-access-with-intune"></a>Intune ile koşullu erişim

Intune ile  **koşullu erişimi**  kullanmak için 3 adım gerekir:

- Cihaz uyumlu olmadan önce karşılanması gereken ayarları tanımlamak için  **Uyumluluk ilkesi**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) oluşturun. Örneğin, bir cihazın uyumlu kabul edilmeden önce en az 6 basamağı olmalıdır.
- Hangi kaynakların korunduğunu ve bu kaynaklara erişmek için hangi koşulların karşılanabileceğini tanımlayan bir **koşullu erişim ilkesi**  oluşturun.  [Örneğin,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  kurumsal e-postaya erişmeden önce bir cihazın uyumlu olması gerekir.
- Hem **uyumluluk ilkeleri**  hem de  **koşullu erişim ilkelerinin**  istenen kullanıcı gruplarını hedeflediğinden emin olun. Bu, Azure Active Directory 'de belirli kullanıcı gruplarını oluşturmanız gerekebilir.

**Faydalı bağlantılar:**

[Cihaz uyumuna genel bakış](https://docs.microsoft.com/intune/device-compliance-get-started)

[Sorun giderme CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Sorun giderme ilkesi](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

E-postayı uyumlu olmayan cihazlara erişimi önlemek için, her iki belgeyi de takip etmelisiniz:

1. [EA kullanarak cihazlardan e-posta erişimini koruma](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Outlook gibi modern kimlik doğrulama istemcileri kullanarak cihazlardan e-posta erişimini koruma](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)