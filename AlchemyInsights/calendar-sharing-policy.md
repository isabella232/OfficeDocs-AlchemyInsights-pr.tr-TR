---
title: 618 Takvim Paylaşımı İlkesi
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091629"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Takvim paylaşımı sırasında ilke hatası

1. Durumunuz için uygun olarak, aşağıdakilerden birini yapın:
    - Bağlan PowerShell Exchange Online powershell kullanarak da bağlanabilirsiniz. Daha fazla bilgi için bkz. Bağlan Uzak [PowerShell Exchange Online'i kullanma hakkında bilgi.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - Şirket içi sunucuda Yönetim Kabuğu'Exchange açın.
2. Kullanıcıya atanan paylaşım ilkeyi belirler. Bunu yapmak için aşağıdaki komutu çalıştırın ve döndürülen ilkeye dikkatin:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Kullanıcının paylaşım ilkesini güncelleştirin. Bunu yapmak için şu adımları uygulayın:
    - Exchange merkezini açın.
    - Kuruluş **'a** tıklayın ve sonra Bireysel Paylaşım altında kullanıcıya atanan ilkeye **çift tıklayın.** Bu, 2. adımda döndürülen ilkedir.
    - Paylaşım Kuralı sayfasında, Paylaşmak istediğiniz bilgileri belirtin altında izin vermek **istediğiniz takvim paylaşım düzeyini seçin;** **Kaydet'e tıklayın.**

Daha fazla bilgi için bkz: Kullanıcı takvimi paylaşmaya çalıştığında "İlke, alıcılardan biri veya birden fazlası için bu düzeyde izinler verilmesine [izin vermiyor" hatası.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
