---
title: 2419-etkin-denetim yapamayan
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510448"
---
# <a name="unable-to-enable-unified-auditing"></a>Birleşik denetimi etkinleştiremiyor

Kuruluşunuz için birleşik denetimi etkinleştirmeye çalıştığınızda, aşağıdakilere benzer bir hata alabilirsiniz:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Bu sorunu gidermek için aşağıdaki adımları izleyin:

1. [Exchange Online Powershell'e bağlanın.](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. Aşağıdaki cmdlet çalıştırın:

   ```
   Enable-OrganizationCustomization
   ```

3. Önceki ayarın etkili olması için 60 dakika bekleyin.

4. Exchange Online PowerShell'de aşağıdaki komutu çalıştırın:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Daha fazla bilgi için aşağıdaki makalelere bakın:

- [Çok faktörlü kimlik doğrulamayı kullanarak Exchange Online PowerShell'e bağlanın](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Denetim günlüğü aramayı açma veya kapatma](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
