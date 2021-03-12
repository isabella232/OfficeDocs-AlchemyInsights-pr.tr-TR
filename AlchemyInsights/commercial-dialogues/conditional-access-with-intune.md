---
title: Intune ile Koşullu Erişim kullanma
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
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749266"
---
# <a name="using-conditional-access-with-intune"></a>Intune ile Koşullu Erişim kullanma

Intune ile Koşullu Erişim'i kullanmak için 3 adım gerekir:

- [Cihazın uyumlu kabul edilene kadar karşılanmayacak ayarları tanımlamak için Uyumluluk İlkesi oluşturun. Örneğin, bir cihazın uyumlu kabul edilirken en az 6 basamaklı bir pin'i olmalıdır.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Korunan kaynakları ve bu kaynaklara erişmek için hangi koşulların karşı korunmasını gerektir olacağını tanımlayan bir Koşullu Erişim İlkesi oluşturun. Örneğin, bir cihaz kurumsal e-postaya erişmeden önce uyumlu olmalıdır.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [İstenen kullanıcı gruplarına hem Uyumluluk İlkelerinin hem de Koşullu Erişim İlkelerinin hedefli olduğundan emin olun. Bunun için Azure Active Directory'de belirli kullanıcı grupları oluşturulması gerekli olabilir.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Daha fazlasını okuyun](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
