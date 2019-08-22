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
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496455"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="25d83-102">Bir kullanıcı posta kutusu paylaşılan bir posta kutusuna Dönüştür</span><span class="sxs-lookup"><span data-stu-id="25d83-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="25d83-103">Kullanıcının Exchange lisansı varsa, kullanıcı posta kutusu yalnızca paylaşılan bir posta kutusuna dönüştürebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="25d83-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="25d83-104">Posta kutusu dönüştürüldükten sonra paylaşılan posta kutuları, liste içerdiğinden etkin kullanıcılar listesinde görünmesi devam edecektir.</span><span class="sxs-lookup"><span data-stu-id="25d83-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="25d83-105">Ancak, dönüştürülmüş posta kutusu ayrıca paylaşılan posta listesinde görünecektir.</span><span class="sxs-lookup"><span data-stu-id="25d83-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="25d83-106">Exchange Yönetim Konsolu'nda posta kutusu dönüştürmeye çalışırsanız ve dönüştürme başarısız olursa, tarayıcı önbelleği ve tanımlama bilgilerini temizleyin ve yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="25d83-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="25d83-107">Hala çalışmıyorsa, posta kutusu Exchange Yönetim Kabuğu'nda aşağıdaki komutu çalıştırarak dönüştürme deneyin:</span><span class="sxs-lookup"><span data-stu-id="25d83-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="25d83-108">Daha fazla posta dönüştürme bilgilerini [bir kullanıcının posta kutusuna paylaşılan bir posta kutusuna dönüştürmek](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox)kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="25d83-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
