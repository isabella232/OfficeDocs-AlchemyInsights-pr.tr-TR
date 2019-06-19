---
title: 2419-oluşturulamıyor-için-enable-denetleme
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065721"
---
# <a name="unable-to-enable-unified-auditing"></a>Birleşik denetim etkinleştirilemiyor

Office 365 kuruluşunuz için birleşik denetimi etkinleştirmeye çalıştığınızda, aşağıdaki benzer bir hata alabilirsiniz:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Bu sorunu gidermek için şu adımları izleyin:

1. [Powershell çevrimiçi alışverişi bağlanın](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Aşağıdaki cmdlet'i çalıştırın:

   ```
   Enable-OrganizationCustomization
   ```

3. Önceki ayarının etkinleşmesi 60 dakika bekleyin.

4. Çevrimiçi Exchange PowerShell içinde aşağıdaki komutu çalıştırın:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Ek bilgi için aşağıdaki makalelere bakın:

- [Exchange Online çok faktörlü kimlik doğrulama kullanarak PowerShell bağlanma](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Office 365 denetim günlüğü aramayı açma veya kapatma](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
