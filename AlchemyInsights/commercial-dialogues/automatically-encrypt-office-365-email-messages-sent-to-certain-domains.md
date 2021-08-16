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
ms.openlocfilehash: 5a285f36aeb814e3b1d361c8cbffd5a6bef0770d10082d24654c7bbda59ce65b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082206"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Belirli etki Office 365 e-posta iletilerini otomatik olarak şifreleme

1. Yönetim merkezinde [Exchange akışı ve](https://outlook.office365.com/ecp/) **kuralları'> seçin.** 
2. Yeni **(+) simgesine** tıklayın ve ardından İletilere **Office 365 İleti Şifrelemesi ve hak koruması uygula'ya tıklayın.**
3. Ad **alanına** kural için, parolaya gönderilen iletileri *şifrele gibi bir contoso.com.*
4. Şu **durumda bu kuralı uygula alanında** **Alıcı, etki > seçin.** 
5. Etki alanının adını girin, örneğin **contoso.com.**
6. Ekle **(+) simgesine** tıklayın ve sonra da Tamam'a **tıklayın.**
7. Aşağıdakini yapın **alanında Birini** seç **'e tıklayın.** 
8. RMS şablonu **açılan menüsünde** Şifrele'yi **seçin ve** Tamam'a **tıklayın.** (Bu seçeneği görmüyorsanız, planınız otomatik şifreleme içermedi demektir. Ancak eklemek de gerekir!)
9. İsteğe bağlı herhangi bir seçimi seçin (bu noktada, bir çoğu basitlik için varsayılan ayarda bırakabilirsiniz) isteğe bağlı seçim listesinden seçim yapın.
10. **Kaydet**'e tıklayın.

> [!IMPORTANT]
> Daha sonra istediğiniz zaman geri gelebilir ve bu kuralı düzenleyebilirsiniz.

Şifreleme kuralları oluşturma hakkında daha fazla bilgi için bkz. [E-posta](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) iletileri şifrelemek için posta akış kurallarını tanımlama Office 365