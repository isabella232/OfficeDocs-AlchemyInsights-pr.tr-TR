---
title: 2419-unable-to-enable-auditing
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
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007810"
---
# <a name="unable-to-enable-unified-auditing"></a>Birleşik denetim etkinleştirilamadi

Organizasyonunız için birleşik denetimi etkinleştirmeye çalışsanız da aşağıdakine benzer bir hata alabilirsiniz:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Bu sorunu çözmek için şu adımları izleyin:

1. [Bağlan Powershell'Exchange Online için yeni bir komutlar.](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. Aşağıdaki cmdlet'i çalıştırın:

   ```
   Enable-OrganizationCustomization
   ```

3. Önceki ayarın yürürlüğe girecek şekilde ayarlaması için 60 dakika bekleyin.

4. Exchange Online PowerShell'de aşağıdaki komutu çalıştırın:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Daha fazla bilgi için aşağıdaki makalelere bakın:

- [Bağlan faktör Exchange Online kullanarak PowerShell'i kullanmaya devam etmek için](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Denetim günlüğü aramalarını açma veya kapatma](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
