---
title: DkIM'i özel etki alanlarıyla ayarlama
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747633"
---
# <a name="set-up-dkim-with-custom-domains"></a>DkIM'i özel etki alanlarıyla ayarlama

DNS'de her özel etki alanı için iki CNAME kaydı yayımlamanız gerekir. Bunu yapmak için aşağıdaki biçimi kullanın:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID,** özel etki alanının özelleştirilmiş MX **kaydında .mail.protection.outlook.com'in** sol tarafından kalan metindir (örneğin, etki alanı yöneticisinin contoso-com **contoso.com).** **InitialDomain,** Office 365'e kayıt olurken kullanılan etki alanıdır (örneğin, contoso.onmicrosoft.com).

DNS kayıtları hakkında daha fazla bilgi için bkz. [Office 365 için herhangi](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)bir DNS barındırma hizmet sağlayıcısında DNS kayıtları oluşturma.