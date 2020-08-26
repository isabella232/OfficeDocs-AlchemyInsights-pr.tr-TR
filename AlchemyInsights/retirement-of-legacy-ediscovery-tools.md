---
title: Eski eBulma araçlarının emekli
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902640"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Eski eBulma araçlarının emekli

Microsoft 365 Uyumluluk Merkezi 'nde yeni ve geliştirilmiş eBulma işlevlerinin sonucu olarak, gelen aylarda aşağıdaki eski eBulma araçları ve Command'in yerine gelmelerini sağlayacaktır:

- Exchange Yönetim merkezinde [yerinde eBulma](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) ve [yerinde saklamalar](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) .

- Yerinde eBulma ve yerinde saklamayı destekleyen Exchange Online PowerShell cmdlet 'leri. (Bu cmdlet 'ler toplu olarak *-MailboxSearch cmdlet 'leri olarak tanımlanır.) Bu, aşağıdaki cmdlet 'leri içerir:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Exchange Online PowerShell 'de [arama-posta kutusu](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet 'i.
- Exchange Web Hizmetleri API 'sinde aşağıdaki işlemler:
    - [Getsearchableposta kutuları](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Setholdonposta kutuları](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Getholdonposta kutuları](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Gelişmiş eBulma v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Emeklilik zaman çizelgesi**:
- **1 temmuz 2020** Artık yeni aramalar ve ayrı tutma oluşturamazsınız, ancak mevcut aramaları kendi sorumluluğunuzdadır, düzenleyebilir ve silebilirsiniz. Microsoft desteği artık EAC 'de sakladıkları & yerinde eBulma desteklemiyor.
    
- **1 ekim 2020** Yerinde eBulma &, EAC 'da ayrı tutma işlevi salt okunur moduna yerleştirilir, dolayısıyla yalnızca var olan aramaları ve ayrı tutmaları kaldırabilirsiniz.

**Daha fazla bilgi için bkz**.

 - [Eski eBulma aramalarını ve bunları Microsoft 365 Uyumluluk Merkezi 'ne geçirme](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Eski eBulma araçlarının emekli](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Yerinde eBulma ve yerinde Saklamalarla ilgili SSS](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



