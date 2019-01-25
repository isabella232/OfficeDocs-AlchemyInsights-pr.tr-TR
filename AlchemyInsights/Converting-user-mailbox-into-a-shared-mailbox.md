---
title: Paylaşılan bir posta uygulamasına dönüştürme kullanıcı posta kutusu?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29494436"
---
Kullanıcının Exchange lisansı varsa, kullanıcı posta kutusu yalnızca paylaşılan bir posta kutusuna dönüştürebilirsiniz. Posta kutusu dönüştürüldükten sonra paylaşılan posta kutuları, liste içerdiğinden etkin kullanıcılar listesinde görünmesi devam edecektir. Ancak, dönüştürülmüş posta kutusu ayrıca paylaşılan posta listesinde görünecektir. 
  
Exchange Yönetim Konsolu'nda posta kutusu dönüştürmeye çalışırsanız ve dönüştürme başarısız olursa, tarayıcı önbelleği ve tanımlama bilgilerini temizleyin ve yeniden deneyin. Hala çalışmıyorsa, posta kutusu Exchange Yönetim Kabuğu'nda aşağıdaki komutu çalıştırarak dönüştürme deneyin:
  
```
Set-Mailbox -Type Shared
```

Daha fazla posta dönüştürme bilgilerini [bir kullanıcının posta kutusuna paylaşılan bir posta kutusuna dönüştürmek](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba)kullanılabilir.
  
