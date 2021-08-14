---
title: Intune ile Koşullu Erişimi kullanma
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005794"
---
# <a name="using-conditional-access-with-intune"></a>Intune ile Koşullu Erişimi kullanma

Intune ile Koşullu Erişimi kullanmak için 3 adım gerekir:

- [Cihazın uyumlu kabul edilene kadar karşılanmalıdır ayarlarını tanımlamak için bir Uyumluluk İlkesi oluşturun. Örneğin, bir cihazın uyumlu kabul edilene kadar en az 6 basamaklı bir PIN kodu olmalıdır.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Korunan kaynakları ve bu kaynaklara erişmek için karşı korunması gereken koşulları tanımlayan bir Koşullu Erişim İlkesi oluşturun. Örneğin, bir cihaz şirket e-postalarına erişmek için uyumlu olmalıdır.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [İstediğiniz kullanıcı gruplarının hem Uyumluluk İlkelerine hem de Koşullu Erişim İlkelerine hedef olduğundan emin olun. Bunun için, çalışma sayfalarında belirli kullanıcı grupları Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Daha fazlasını okuyun](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
