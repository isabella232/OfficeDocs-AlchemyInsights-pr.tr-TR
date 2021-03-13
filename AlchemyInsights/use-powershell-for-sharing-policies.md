---
title: Paylaşım ilkeleri ve Organizasyon İlişkileri için Windows PowerShell'i kullanma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709486"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="eafd0-102">Paylaşım ilkeleri ve Organizasyon İlişkileri için Windows PowerShell'i kullanma</span><span class="sxs-lookup"><span data-stu-id="eafd0-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="eafd0-103">Organizasyon ilişkileri için lütfen ayrıntılı söz dizimini ve aşağıdakiler için parametre bilgilerini inceleyin: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  VE  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="eafd0-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="eafd0-104">Paylaşım ilkesi oluşturmak için [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy)'ı kullanın.</span><span class="sxs-lookup"><span data-stu-id="eafd0-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="eafd0-105">[Bir posta kutusuna veya kullanıcıya paylaşım ilkesi uygulamak](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) için yeni oluşturulan ilke ile [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) ve [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) birleşimini kullanın.</span><span class="sxs-lookup"><span data-stu-id="eafd0-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="eafd0-106">[Bir paylaşım ilkesini düzenlemek, devre dışı bırakmak veya kaldırmak için](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ve [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)'ı kullanmanız gerekiyor.</span><span class="sxs-lookup"><span data-stu-id="eafd0-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="eafd0-107">**Bu konuyu tam olarak anlamak için lütfen aşağıdakini okuyun:**</span><span class="sxs-lookup"><span data-stu-id="eafd0-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="eafd0-108">Exchange Online'da paylaşım</span><span class="sxs-lookup"><span data-stu-id="eafd0-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)