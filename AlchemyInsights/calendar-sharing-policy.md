---
title: 618 Takvim Paylaşım Politikası
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373019"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Takvim paylaşırken ilke hatası

1. Durumunuza uygun olarak aşağıdakilerden birini yapın:
    - Remote PowerShell'i kullanarak Exchange Online'a bağlanın. Daha fazla bilgi için Remote [PowerShell kullanarak Exchange Online'a Bağlan'a](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)bakın.
    - Şirket içi sunucuda Exchange Management Shell'i açın.
2. Kullanıcıya atanan paylaşım ilkesini belirleyin. Bunu yapmak için aşağıdaki komutu çalıştırın ve döndürülen ilkeyi not edin:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Kullanıcı için paylaşım ilkesini güncelleştirin. Bunu yapmak için aşağıdaki adımları izleyin:
    - Exchange yönetici merkezini açın.
    - **Kuruluş'u**tıklatın ve ardından **Bireysel Paylaşım**altında kullanıcıya atanan ilkeyi çift tıklatın. Bu, adım 2'de döndürülen ilkedir.
    - Paylaşım Kuralı sayfasında, hangi **bilgileri paylaşmak istediğinizi belirt' in**altında izin vermek istediğiniz takvim paylaşım düzeyini seçin; **kaydet'i**tıklatın.

Daha fazla bilgi için bkz: ["İlke, kullanıcı takvimi paylaşmaya çalıştığında bu düzeyde bir veya daha fazla alıcıya izin verilmesine izin vermez.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
