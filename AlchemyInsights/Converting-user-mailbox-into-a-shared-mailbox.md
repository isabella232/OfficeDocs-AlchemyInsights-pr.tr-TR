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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28318402"
---
<span data-ttu-id="22cc4-p101">Kullanıcının Exchange lisansı varsa, kullanıcı posta kutusu yalnızca paylaşılan bir posta kutusuna dönüştürebilirsiniz. Posta kutusu dönüştürüldükten sonra paylaşılan posta kutuları, liste içerdiğinden etkin kullanıcılar listesinde görünmesi devam edecektir. Ancak, dönüştürülmüş posta kutusu ayrıca paylaşılan posta listesinde görünecektir.</span><span class="sxs-lookup"><span data-stu-id="22cc4-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="22cc4-p102">Exchange Yönetim Konsolu'nda posta kutusu dönüştürmeye çalışırsanız ve dönüştürme başarısız olursa, tarayıcı önbelleği ve tanımlama bilgilerini temizleyin ve yeniden deneyin. Hala çalışmıyorsa, posta kutusu Exchange Yönetim Kabuğu'nda aşağıdaki komutu çalıştırarak dönüştürme deneyin:</span><span class="sxs-lookup"><span data-stu-id="22cc4-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="22cc4-107">Daha fazla posta dönüştürme bilgilerini [bir kullanıcının posta kutusuna paylaşılan bir posta kutusuna dönüştürmek](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba)kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="22cc4-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
