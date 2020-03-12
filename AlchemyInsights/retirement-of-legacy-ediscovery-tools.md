---
title: Legacy eDiscovery Araçları emeklilik
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
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600404"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Legacy eDiscovery Araçları emeklilik

Microsoft 365 Uyumluluk merkezindeki yeni ve geliştirilmiş eDiscovery işlevinin bir sonucu olarak, aşağıdaki eski eDiscovery araçları ve komutları önümüzdeki aylarda kullanımdan kaldırılacaktır:

- Exchange yönetici merkezinde [yer-in-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) ve [Yerinde Tutar.](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)

- Yerinde eDiscovery ve Yerinde Tutar destekleyen Exchange Online PowerShell cmdlets. (Bu cmdletler topluca *-MailboxSearch cmdlets olarak tanımlanır.) Bu aşağıdaki cmdlets içerir:

    - [Yeni Posta KutusuArama](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Başlangıç-Posta KutusuArama](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxArama](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxArama](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Exchange Online PowerShell [arama-posta kutusu](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet.
- Exchange Web Hizmetleri API'sında aşağıdaki işlemler:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 Gelişmiş eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Emeklilik için zaman çizelgesi:**
- 1 Nisan 2020: Yeni aramalar ve tutarlar oluşturamazsınız, ancak varolan aramaları kendi riskiniz altında çalıştırabilir, düzenleyebilir ve silebilirsiniz. Microsoft Desteği artık EAC'de bulunan & Yerinde eDiscovery'yi desteklemez.

- 1 Temmuz 2020: EAC'de barındıran Yerinde eDiscovery & Yalnızca Okunur modunda yerleştirilecektir. Bu, yalnızca varolan aramaları ve aramaları kaldırabileceğiniz anlamına gelir.

**Daha fazla bilgi için bkz:**

 - [Eski eDiscovery aramalarını ve Microsoft 365 uyumluluk merkezine geçiş yapmayı](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Eski eDiscovery araçlarının emekliliği](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Yerinde eDiscovery ve Yerinde Tutarlar hakkında SSS](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



