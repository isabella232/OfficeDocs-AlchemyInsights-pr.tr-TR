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
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704806"
---
# <a name="conditional-access-with-intune"></a>Intune ile Koşullu Erişim

**Intune** ile Koşullu Erişim'i kullanmak için 3 adım gerekir:

- Cihazın uyumlu  **kabul edilene**  kadar karşılanmayacak ayarları tanımlamak için Uyumluluk İlkesi [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)oluşturun. Örneğin, bir cihazın uyumlu kabul edilene kadar en az 6 basamaklı bir pin'i olmalıdır.
- Korunan **kaynakları ve bu**  kaynaklara erişmek için hangi koşulların karşı korunmasını gerektir olacağını tanımlayan bir Koşullu Erişim İlkesi oluşturun.  [Örneğin, bir cihaz](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  kurumsal e-postaya erişmeden önce uyumlu olmalıdır.
- İstenen kullanıcı **gruplarına**  hem  **Uyumluluk İlkelerinin**  hem de Koşullu Erişim İlkelerinin hedefli olduğundan emin olun. Bunun için Azure Active Directory'de belirli kullanıcı grupları oluşturulması gerekli olabilir.

**Yararlı bağlantılar:**

[Cihaz uyumluluğuna genel bakış](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA sorunlarını giderme](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Sorun giderme ilkesi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Uyumlu olmayan cihazlar tarafından E-postayı (Exchange Online) erişime karşı korumak için her iki belge de izlenmektedir:

1. [EAS kullanarak cihazlardan e-posta erişimini koruma](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Outlook gibi modern kimlik doğrulama istemcilerini kullanarak cihazlardan e-posta erişimini koruma](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)