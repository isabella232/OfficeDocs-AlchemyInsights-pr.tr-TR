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
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798569"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="057a4-102">Eski eBulma Araçları'nın eskiden emeklilik</span><span class="sxs-lookup"><span data-stu-id="057a4-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="057a4-103">Microsoft 365 Uyumluluk merkezi'nde yeni ve geliştirilmiş eKbulma işlevselliğinin bir sonucu olarak, önümüzdeki aylarda aşağıdaki eski eBulma araçları ve komutlar kullanımdan kaldıracak:</span><span class="sxs-lookup"><span data-stu-id="057a4-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="057a4-104">Exchange yönetim merkezinde Yerinde [eKbulma ve Yerinde 1](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) 6/ 1. [](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)</span><span class="sxs-lookup"><span data-stu-id="057a4-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="057a4-105">e In-Place Bulma ve 1 1 1 7/2 In-Place Exchange Online PowerShell cmdlet'leri.</span><span class="sxs-lookup"><span data-stu-id="057a4-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="057a4-106">(Bu cmdlet'ler toplu olarak \*-MailboxSearch cmdlet'leri olarak tanımlanır.) Bu cmdlet'ler şunları içerir:</span><span class="sxs-lookup"><span data-stu-id="057a4-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="057a4-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="057a4-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="057a4-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="057a4-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="057a4-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="057a4-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="057a4-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="057a4-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="057a4-111">Exchange Online [PowerShell'de Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet'i.</span><span class="sxs-lookup"><span data-stu-id="057a4-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="057a4-112">Exchange Web Hizmetleri API'sinde aşağıdaki işlemler:</span><span class="sxs-lookup"><span data-stu-id="057a4-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="057a4-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="057a4-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="057a4-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="057a4-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="057a4-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="057a4-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="057a4-116">Gelişmiş eKbulma v1.0</span><span class="sxs-lookup"><span data-stu-id="057a4-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="057a4-117">**Emeklilik için zaman çizelgesi:**</span><span class="sxs-lookup"><span data-stu-id="057a4-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="057a4-118">**1 Temmuz 2020** Artık yeni arama ve uzamaz, ancak var olan aramaları çalıştırmak, düzenlemek ve silmek size aittir.</span><span class="sxs-lookup"><span data-stu-id="057a4-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="057a4-119">Microsoft Desteği artık EAC'In-Place eK bulma ve 1& 1.</span><span class="sxs-lookup"><span data-stu-id="057a4-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="057a4-120">**1 Ekim 2020** In-Place EAC'de eBulma & 12 Ekim 2013'te salt okunur moda yerleştirilsin, böylece yalnızca var olan aramaları ve 1.</span><span class="sxs-lookup"><span data-stu-id="057a4-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="057a4-121">**Daha fazla bilgi için bkz:**</span><span class="sxs-lookup"><span data-stu-id="057a4-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="057a4-122">Eski eBulma aramalarını ve 365 uyumluluk merkezine geçirme</span><span class="sxs-lookup"><span data-stu-id="057a4-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="057a4-123">Eski eBulma araçlarının emeklilik</span><span class="sxs-lookup"><span data-stu-id="057a4-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="057a4-124">eBulma ve In-Place Hakkında SSS In-Place SSS</span><span class="sxs-lookup"><span data-stu-id="057a4-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



