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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="0585f-102">Legacy eDiscovery Araçları emeklilik</span><span class="sxs-lookup"><span data-stu-id="0585f-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="0585f-103">Microsoft 365 Uyumluluk merkezindeki yeni ve geliştirilmiş eDiscovery işlevinin bir sonucu olarak, aşağıdaki eski eDiscovery araçları ve komutları önümüzdeki aylarda kullanımdan kaldırılacaktır:</span><span class="sxs-lookup"><span data-stu-id="0585f-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="0585f-104">Exchange yönetici merkezinde [yer-in-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) ve [Yerinde Tutar.](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)</span><span class="sxs-lookup"><span data-stu-id="0585f-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="0585f-105">Yerinde eDiscovery ve Yerinde Tutar destekleyen Exchange Online PowerShell cmdlets.</span><span class="sxs-lookup"><span data-stu-id="0585f-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="0585f-106">(Bu cmdletler topluca \*-MailboxSearch cmdlets olarak tanımlanır.) Bu aşağıdaki cmdlets içerir:</span><span class="sxs-lookup"><span data-stu-id="0585f-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="0585f-107">Yeni Posta KutusuArama</span><span class="sxs-lookup"><span data-stu-id="0585f-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="0585f-108">Başlangıç-Posta KutusuArama</span><span class="sxs-lookup"><span data-stu-id="0585f-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="0585f-109">Stop-MailboxArama</span><span class="sxs-lookup"><span data-stu-id="0585f-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="0585f-110">Set-MailboxArama</span><span class="sxs-lookup"><span data-stu-id="0585f-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="0585f-111">Exchange Online PowerShell [arama-posta kutusu](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet.</span><span class="sxs-lookup"><span data-stu-id="0585f-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="0585f-112">Exchange Web Hizmetleri API'sında aşağıdaki işlemler:</span><span class="sxs-lookup"><span data-stu-id="0585f-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="0585f-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="0585f-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="0585f-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="0585f-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="0585f-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="0585f-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="0585f-116">Office 365 Gelişmiş eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="0585f-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="0585f-117">**Emeklilik için zaman çizelgesi:**</span><span class="sxs-lookup"><span data-stu-id="0585f-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="0585f-118">1 Nisan 2020: Yeni aramalar ve tutarlar oluşturamazsınız, ancak varolan aramaları kendi riskiniz altında çalıştırabilir, düzenleyebilir ve silebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0585f-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="0585f-119">Microsoft Desteği artık EAC'de bulunan & Yerinde eDiscovery'yi desteklemez.</span><span class="sxs-lookup"><span data-stu-id="0585f-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="0585f-120">1 Temmuz 2020: EAC'de barındıran Yerinde eDiscovery & Yalnızca Okunur modunda yerleştirilecektir.</span><span class="sxs-lookup"><span data-stu-id="0585f-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="0585f-121">Bu, yalnızca varolan aramaları ve aramaları kaldırabileceğiniz anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="0585f-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="0585f-122">**Daha fazla bilgi için bkz:**</span><span class="sxs-lookup"><span data-stu-id="0585f-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="0585f-123">Eski eDiscovery aramalarını ve Microsoft 365 uyumluluk merkezine geçiş yapmayı</span><span class="sxs-lookup"><span data-stu-id="0585f-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="0585f-124">Eski eDiscovery araçlarının emekliliği</span><span class="sxs-lookup"><span data-stu-id="0585f-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="0585f-125">Yerinde eDiscovery ve Yerinde Tutarlar hakkında SSS</span><span class="sxs-lookup"><span data-stu-id="0585f-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



