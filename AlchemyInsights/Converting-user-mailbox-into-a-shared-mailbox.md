---
title: Paylaşılan bir posta uygulamasına dönüştürme kullanıcı posta kutusu?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374343"
---
<span data-ttu-id="202cd-102">Kullanıcının Exchange lisansı varsa, kullanıcı posta kutusu yalnızca paylaşılan bir posta kutusuna dönüştürebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="202cd-102">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="202cd-103">Posta kutusu dönüştürüldükten sonra paylaşılan posta kutuları, liste içerdiğinden etkin kullanıcılar listesinde görünmesi devam edecektir.</span><span class="sxs-lookup"><span data-stu-id="202cd-103">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="202cd-104">Ancak, dönüştürülmüş posta kutusu ayrıca paylaşılan posta listesinde görünecektir.</span><span class="sxs-lookup"><span data-stu-id="202cd-104">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="202cd-105">Exchange Yönetim Konsolu'nda posta kutusu dönüştürmeye çalışırsanız ve dönüştürme başarısız olursa, tarayıcı önbelleği ve tanımlama bilgilerini temizleyin ve yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="202cd-105">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="202cd-106">Hala çalışmıyorsa, posta kutusu Exchange Yönetim Kabuğu'nda aşağıdaki komutu çalıştırarak dönüştürme deneyin:</span><span class="sxs-lookup"><span data-stu-id="202cd-106">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="202cd-107">Daha fazla posta dönüştürme bilgilerini [bir kullanıcının posta kutusuna paylaşılan bir posta kutusuna dönüştürmek](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba)kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="202cd-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
