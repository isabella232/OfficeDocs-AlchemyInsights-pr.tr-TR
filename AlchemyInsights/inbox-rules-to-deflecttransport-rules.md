---
title: DeflectTransport kuralları 929 gelen kutusu kuralları
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/15/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 929
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 9b78dea8557c68d23cf1409ebd6f7c7aab46f1be
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776871"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="f2c53-102">Posta akışı kuralları (aktarım kuralları olarak da bilinir)</span><span class="sxs-lookup"><span data-stu-id="f2c53-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="f2c53-103">Posta akışı kuralları genel bakış: [posta akışı kuralları (taşıma kuralları) Exchange çevrimiçi](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="f2c53-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>
    
- <span data-ttu-id="f2c53-104">Posta akışı kuralları Kurulumu: [posta akış yordamları kural Exchange çevrimiçi](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="f2c53-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>
    
- <span data-ttu-id="f2c53-105">Oluşturma, değiştirme ve silme posta akışı kuralları: [posta akışı kuralları Yönet](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="f2c53-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>
    
<span data-ttu-id="f2c53-106">Posta akışı kuralları çevrimiçi PowerShell Exchange de yönetebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f2c53-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="f2c53-107">Daha fazla bilgi için bkz: [Get TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (Görünüm), [Yeni TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (Oluştur) [TransportRule kaldırma](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (silme), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (değiştirmek varolan), (devre dışı bırakma varolan) [Devre dışı bırakma-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) ve [TransportRule etkinleştir](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (varolan etkinleştir).</span><span class="sxs-lookup"><span data-stu-id="f2c53-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span> 
  
<span data-ttu-id="f2c53-108">Ek posta akışı kural cmdlet'leri: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (liste kullanılabilir eylemler), [Al-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (liste kullanılabilir koşullar ve özel durumlar), [Verme TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (İhracat Kuralları) ve [ Al-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (kuralları Al).</span><span class="sxs-lookup"><span data-stu-id="f2c53-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span> 
  

