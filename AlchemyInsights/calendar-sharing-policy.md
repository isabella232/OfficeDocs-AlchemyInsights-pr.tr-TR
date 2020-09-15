---
title: 618 takvim paylaşım Ilkesi
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
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684250"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Takvim paylaşırken ilke hatası

1. Aşağıdakilerden birini yapın:
    - Uzak PowerShell 'i kullanarak Exchange Online 'a bağlanın. Daha fazla bilgi için, [uzak PowerShell kullanarak Exchange Online 'A bağlanın](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Şirket içi sunucuda Exchange Yönetim Kabuğu 'nu açın.
2. Kullanıcıya atanan paylaşım ilkesini belirleme. Bunu yapmak için, aşağıdaki komutu çalıştırıp verilen ilkeye dikkat edin:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Kullanıcının paylaşım ilkesini güncelleyin. Bunu yapmak için şu adımları uygulayın:
    - Exchange Yönetim merkezini açın.
    - **Kuruluş**'a tıklayın ve ardından **bireysel paylaşım**altında kullanıcıya atanmış olan ilkeye çift tıklayın. Bu, adım 2 ' de döndürülen ilkedir.
    - Paylaşım kuralı sayfasında, izin vermek istediğiniz takvim paylaşım düzeyini **paylaşmak istediğiniz bilgileri belirtip**seçin; **Kaydet**'e tıklayın.

Daha fazla bilgi için, [Kullanıcı takvimi paylaşmaya çalışıldığında "ilke bu düzeyde bir veya birden çok alıcıya izin vermeye izin vermiyor" hatasını](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)inceleyin.
