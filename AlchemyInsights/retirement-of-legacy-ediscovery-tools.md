---
title: Eski eBulma Araçları'nın eskiden emeklilik
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074700"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Eski eBulma Araçları'nın eskiden emeklilik

Microsoft 365 Uyumluluk Merkezi'nde yeni ve geliştirilmiş eKbulma işlevselliğinin sonucunda, önümüzdeki aylarda aşağıdaki eski eBulma araçları ve komutlar kullanımdan kaldıracak:

- [Yönetim merkezinde Yerinde eKbulma](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [ve Yerinde 1](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Exchange 1.

- eK Exchange Online 7/ In-Place 2 /c0 "1" desteği olan In-Place PowerShell cmdlet'leridir. (Bu cmdlet'ler toplu olarak *-MailboxSearch cmdlet'leri olarak tanımlanır.) Bu cmdlet'ler şunları içerir:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Exchange Online PowerShell'de [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet'i.
- Exchange Web Hizmetleri API'sinde aşağıdaki işlemler:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Emeklilik için zaman çizelgesi:**
- **1 Temmuz 2020** Artık yeni arama ve uzamaz, ancak var olan aramaları çalıştırmak, düzenlemek ve silmek size aittir. Microsoft Desteği artık EAC'In-Place eK bulma ve 1& 1.
    
- **1 Ekim 2020** In-Place EAC'de eBulma & 12 Ekim 2013'te salt okunur moda yerleştirilsin, böylece yalnızca var olan aramaları ve 1.

**Daha fazla bilgi için bkz:**

 - [Eski eBulma aramalarını ve Microsoft 365 uyumluluk merkezi 10.](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Eski eBulma araçlarının emeklilik](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [eBulma ve In-Place Hakkında SSS In-Place SSS](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



