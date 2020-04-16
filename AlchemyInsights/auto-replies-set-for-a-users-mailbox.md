---
title: Posta kutusu için otomatik yanıtları ayarlama
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509537"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Kullanıcının posta kutusu için otomatik yanıtları ayarlama

**1. Yöntem**

1. Office 365 portalında oturum açın.

2. **Kullanıcılar > Etkin kullanıcılar**’a (veya paylaşılan posta kutusunda ayarlıyorsanız **Gruplar > Paylaşılan posta kutuları**’na) gidin.

3. Microsoft Exchange posta kutusu olan bir kullanıcı seçin.

4. Sağ taraftaki açılır menüde **Posta ayarları > Otomatik yanıtlar**’a gidin (paylaşılan posta kutusu söz konusuysa açılır menüde doğrudan **Otomatik yanıtlar**’a tıklayın).

**2. Yöntem**

1. Yönetici kimlik bilgilerini kullanarak Office 365 yönetim portalında oturum açın.

2. **Yönetim Merkezleri**’ni genişletin ve sonra **Exchange**’e tıklayın.

3. Sağ üst köşedeki resme tıklayın, **Başka Kullanıcı**’ya tıklayın ve değiştirmek istediğiniz kullanıcı posta kutusunu seçin.

4. Sol tarafta **Seçenekler**’i seçin, **E-postayı Düzenle**’ye ve sonra da **Otomatik yanıtlar**’a tıklayın.

**3. Yöntem**

Exchange Online PowerShell’de şu cmdlet’i çalıştırın:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Bu cmdlet hakkında daha fazla bilgi için bkz. [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
