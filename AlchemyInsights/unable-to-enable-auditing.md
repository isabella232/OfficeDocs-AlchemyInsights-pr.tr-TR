---
title: 2419-etkinleştirme yapılamıyor-denetim
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767619"
---
# <a name="unable-to-enable-unified-auditing"></a>Birleşik denetim etkinleştirilemiyor

Kuruluşunuz için Birleşik denetimi etkinleştirmeye çalıştığınızda, aşağıdakine benzer bir hata alabilirsiniz:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Bu sorunu çözmek için aşağıdaki adımları izleyin:

1. [Exchange Online PowerShell 'e bağlanın](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Aşağıdaki cmdlet 'i çalıştırın:

   ```
   Enable-OrganizationCustomization
   ```

3. Önceki ayarın geçerlilik kazanması için 60 dakika bekleyin.

4. Exchange Online PowerShell 'de aşağıdaki komutu çalýþtýrýn:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Ek bilgi için aşağıdaki makalelere bakın:

- [Multi-Factor Authentication kullanarak Exchange Online PowerShell 'e bağlanma](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Denetim günlüğü aramasını açma veya kapatma](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
