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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="22747-102">Eski eBulma araçlarının emekli</span><span class="sxs-lookup"><span data-stu-id="22747-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="22747-103">Microsoft 365 Uyumluluk Merkezi 'nde yeni ve geliştirilmiş eBulma işlevlerinin sonucu olarak, gelen aylarda aşağıdaki eski eBulma araçları ve Command'in yerine gelmelerini sağlayacaktır:</span><span class="sxs-lookup"><span data-stu-id="22747-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="22747-104">Exchange Yönetim merkezinde [yerinde eBulma](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) ve [yerinde saklamalar](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) .</span><span class="sxs-lookup"><span data-stu-id="22747-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="22747-105">Yerinde eBulma ve yerinde saklamayı destekleyen Exchange Online PowerShell cmdlet 'leri.</span><span class="sxs-lookup"><span data-stu-id="22747-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="22747-106">(Bu cmdlet 'ler toplu olarak \*-MailboxSearch cmdlet 'leri olarak tanımlanır.) Bu, aşağıdaki cmdlet 'leri içerir:</span><span class="sxs-lookup"><span data-stu-id="22747-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="22747-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="22747-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="22747-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="22747-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="22747-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="22747-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="22747-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="22747-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="22747-111">Exchange Online PowerShell 'de [arama-posta kutusu](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet 'i.</span><span class="sxs-lookup"><span data-stu-id="22747-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="22747-112">Exchange Web Hizmetleri API 'sinde aşağıdaki işlemler:</span><span class="sxs-lookup"><span data-stu-id="22747-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="22747-113">Getsearchableposta kutuları</span><span class="sxs-lookup"><span data-stu-id="22747-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="22747-114">Setholdonposta kutuları</span><span class="sxs-lookup"><span data-stu-id="22747-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="22747-115">Getholdonposta kutuları</span><span class="sxs-lookup"><span data-stu-id="22747-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="22747-116">Gelişmiş eBulma v 1.0</span><span class="sxs-lookup"><span data-stu-id="22747-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="22747-117">**Emeklilik zaman çizelgesi**:</span><span class="sxs-lookup"><span data-stu-id="22747-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="22747-118">**1 temmuz 2020** Artık yeni aramalar ve ayrı tutma oluşturamazsınız, ancak mevcut aramaları kendi sorumluluğunuzdadır, düzenleyebilir ve silebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="22747-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="22747-119">Microsoft desteği artık EAC 'de sakladıkları & yerinde eBulma desteklemiyor.</span><span class="sxs-lookup"><span data-stu-id="22747-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="22747-120">**1 ekim 2020** Yerinde eBulma &, EAC 'da ayrı tutma işlevi salt okunur moduna yerleştirilir, dolayısıyla yalnızca var olan aramaları ve ayrı tutmaları kaldırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="22747-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="22747-121">**Daha fazla bilgi için bkz**.</span><span class="sxs-lookup"><span data-stu-id="22747-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="22747-122">Eski eBulma aramalarını ve bunları Microsoft 365 Uyumluluk Merkezi 'ne geçirme</span><span class="sxs-lookup"><span data-stu-id="22747-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="22747-123">Eski eBulma araçlarının emekli</span><span class="sxs-lookup"><span data-stu-id="22747-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="22747-124">Yerinde eBulma ve yerinde Saklamalarla ilgili SSS</span><span class="sxs-lookup"><span data-stu-id="22747-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



