---
title: DeflectTransport kuralları 929 gelen kutusu kuralları
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/15/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 140cb6e85d0f08393439b023578457998a84dc62
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36499623"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="c3fbf-102">Posta akışı kuralları (aktarım kuralları olarak da bilinir)</span><span class="sxs-lookup"><span data-stu-id="c3fbf-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="c3fbf-103">Posta akışı kuralları genel bakış: [posta akışı kuralları (taşıma kuralları) Exchange çevrimiçi](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="c3fbf-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="c3fbf-104">Posta akışı kuralları Kurulumu: [posta akış yordamları kural Exchange çevrimiçi](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="c3fbf-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="c3fbf-105">Oluşturma, değiştirme ve silme posta akışı kuralları: [posta akışı kuralları Yönet](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="c3fbf-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="c3fbf-106">Posta akışı kuralları çevrimiçi PowerShell Exchange de yönetebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c3fbf-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="c3fbf-107">Daha fazla bilgi için bkz: [Get TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (Görünüm), [Yeni TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (Oluştur) [TransportRule kaldırma](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (silme), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (değiştirmek varolan), (devre dışı bırakma varolan) [Devre dışı bırakma-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) ve [TransportRule etkinleştir](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (varolan etkinleştir).</span><span class="sxs-lookup"><span data-stu-id="c3fbf-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="c3fbf-108">Ek posta akışı kural cmdlet'leri: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (liste kullanılabilir eylemler), [Al-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (liste kullanılabilir koşullar ve özel durumlar), [Verme TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (İhracat Kuralları) ve [ Al-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (kuralları Al).</span><span class="sxs-lookup"><span data-stu-id="c3fbf-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
