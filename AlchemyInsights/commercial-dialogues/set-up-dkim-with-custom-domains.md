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
ms.openlocfilehash: bb19f0672a21ea8b99c433ad83db4d89536c9a1705245fd2a683471170ab51ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994849"
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
> **DomainGUID,** özel etki alanı için özelleştirilmiş MX kaydında **.mail.protection.outlook.com'in** sol tarafta yer alan metindir (örneğin, etki alanı yöneticisi için contoso-com **contoso.com).** **InitialDomain,** etki alanı için kayıt olurken Office 365 etki alanıdır (örneğin, **contoso.onmicrosoft.com).**

DNS kayıtları hakkında daha fazla bilgi için bkz. Dns kayıtları için herhangi [bir DNS barındırma sağlayıcısında DNS Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)