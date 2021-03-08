---
title: Belirli etki alanlarına gönderilen Office 365 e-posta iletilerini otomatik olarak şifreleme
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527598"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Belirli etki alanlarına gönderilen Office 365 e-posta iletilerini otomatik olarak şifreleme

1. Exchange yönetim [merkezinde posta](https://outlook.office365.com/ecp/)akışı yönetim **> seçin.** 
2. Yeni **(+) simgesine** tıklayın ve sonra iletilere **Office 365 İleti Şifrelemesi ve hak koruması uygula'ya tıklayın.**
3. Ad **alanına** kural için bir ad girin; örneğin, *E-postaya gönderilen iletileri contoso.com.*
4. Bu **kuralı uygula alanında, etki** alanının alıcı > **seçin.** 
5. Etki alanının adını girin, örneğin **contoso.com.**
6. Ekle **(+) simgesine** ve ardından Tamam'a **tıklayın.**
7. Aşağıdaki do **alanını yanında, Birini** **seç'i tıklatın.** 
8. RMS şablonu **açılan menüsünde** Şifrele'yi seçin **ve** Tamam'a **tıklayın.** (Bu seçeneği görmüyorsanız, planınız otomatik şifreleme içermesi anlamına gelir. Ancak add it!)
9. İsteğe bağlı herhangi bir seçim seçin (bu noktada, çoğu basitlik için varsayılan ayarla bırakıla birlikte bırakabilirsiniz) isteğe bağlı seçimler listesinden seçim yapın.
10. **Kaydet**’e tıklayın.

> [!IMPORTANT]
> Daha sonra istediğiniz zaman geri gelebilir ve bu kuralı düzenleyebilirsiniz.

Şifreleme kuralları oluşturma hakkında daha fazla bilgi için, [Office 365'te](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) e-posta iletilerini şifrelemek için posta akışı kurallarını tanımlama