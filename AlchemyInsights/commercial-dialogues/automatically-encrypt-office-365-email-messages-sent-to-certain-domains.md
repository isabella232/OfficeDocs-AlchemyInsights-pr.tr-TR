---
title: Belirli etki Office 365 e-posta iletilerini otomatik olarak şifreleme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: d30535d8605fcbfa0ca73c262d8f8671d73234a4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318868"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Belirli etki Office 365 e-posta iletilerini otomatik olarak şifreleme

1. Yönetim merkezinde [Exchange akışı](https://outlook.office365.com/ecp/)ve **kuralları'> seçin.** 
2. Yeni **(+) simgesine tıklayın** ve ardından İletilere Office 365 İleti Şifrelemesi **ve hak koruması uygula'ya tıklayın.**
3. Ad **alanına** kural için, parolaya gönderilen iletileri *şifrele gibi bir contoso.com.*
4. Şu **durumda bu kuralı uygula alanında** Alıcı etki > **seçin.** 
5. Etki alanının adını girin, örneğin **contoso.com.**
6. Ekle **(+) simgesine** tıklayın ve sonra da Tamam'a **tıklayın.**
7. Aşağıdakini yapın **alanında Birini** seç **'e tıklayın.** 
8. RMS şablonu **açılan menüsünde** Şifrele'yi **seçin ve** Tamam'a **tıklayın.** (Bu seçeneği görmüyorsanız, planınız otomatik şifreleme içermedi demektir. Ancak eklemek de gerekir!)
9. İsteğe bağlı herhangi bir seçimi seçin (bu noktada seçebiliyorsanız, çoğu basitlik için varsayılan ayarda bırakabilirsiniz) isteğe bağlı seçim listesinden seçim yapın.
10. **Kaydet**'e tıklayın.

**Önemli:** Her zaman geri gelebilir ve bu kuralı daha sonra düzenleyebilirsiniz.

Şifreleme kuralları oluşturma hakkında daha fazla bilgi için bkz. [E-posta](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) iletileri şifrelemek için posta akış kurallarını tanımlama Office 365