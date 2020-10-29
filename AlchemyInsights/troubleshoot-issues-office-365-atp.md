---
title: Office için Microsoft Defender 365 (ATP) sorunlarını giderme
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801427"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Office 365 ATP ile ilgili sorunları giderme

- **E-posta iletisi tesliminde gecikmeler fark** edilsin mi? ATP güvenli ekler ilkeleriniz için dinamik teslim seçeneğini kullanmayı deneyin. Bu, alıcıları kötü niyetli dosyalardan korurken e-posta iletisi gönderme gecikmelerini engellemez.
- **Yanlış pozitif durumları veya yanlış negatifleri raporlamak** mi istiyorsunuz? Dosyanızı çözümleme için göndermek üzere bu bağlantıyı kullanın: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Kuruluşunuzdaki kişilerin gönderdiği e-posta IÇIN ATP güvenli bağlantılar korumasını etkinleştirebildiğinizi biliyor muydunuz** ? Şu adımları izleyin:
    1. Gidin https://protection.office.com ve oturum açın.
    2. **Tehdit yönetimi**  >  **ilkesi**  >  **güvenli bağlantılarına** gidin.
    3. **Belirli alıcılara uygulanan ilkeler** altında, bir ilkeyi düzenleyin (veya ekleyin).
    4. **Kuruluş içinde gönderilen iletilere güvenli bağlantılar Uygula** seçeneğini belirleyin.
    5. İlkenizi kaydedin ve değişikliklerinizin veri merkezinize göre çalışmasını sağlamak için 30 dakikalık bir izin verin.
- ATP ile ilgili daha fazla yardım almak için [Office 365 Için Microsoft Defender](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)'a bakın.