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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332327"
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
**Not:** **DomainGUID,** özel etki alanının özelleştirilmiş MX kaydında **.mail.protection.outlook.com'in** sol tarafta yer alan metindir (örneğin, etki alanı için contoso-com **contoso.com).** **InitialDomain,** etki alanına (örneğin, Office 365) için kayıt olurken **contoso.onmicrosoft.com.**

DNS kayıtları hakkında daha fazla bilgi için bkz. Dns kayıtları için herhangi [bir DNS barındırma Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)