---
title: İlkeleri ve Kuruluş ilişkilerini paylaşmak için PowerShell'i kullanma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862159"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="b9112-102">İlkeleri ve Kuruluş ilişkilerini paylaşmak için PowerShell'i kullanma</span><span class="sxs-lookup"><span data-stu-id="b9112-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="b9112-103">Organizasyon ilişkileri için lütfen detaylı sözdizimi ve parametre bilgilerini gözden geçirin: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) AND [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="b9112-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="b9112-104">Paylaşım ilkesi oluşturmak için [Yeni Paylaşım Politikası'nı](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy)kullanın.</span><span class="sxs-lookup"><span data-stu-id="b9112-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="b9112-105">[Bir posta kutusuna veya kullanıcıya paylaşım ilkesi uygulamak için,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) yeni oluşturulan ilkeyle [Set-Posta Kutusu](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) ve [Get-Mailbox'ın](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) birleşimini kullanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="b9112-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="b9112-106">[Bir paylaşım ilkesini değiştirmek, devre dışı kaldırıp kaldırmak](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) için [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ve [Remove-SharingPolicy'yi](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)kullanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="b9112-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="b9112-107">**Bu konunun tam olarak anlaşılması için lütfen okuyun:**</span><span class="sxs-lookup"><span data-stu-id="b9112-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="b9112-108">Exchange Online'da Paylaşım</span><span class="sxs-lookup"><span data-stu-id="b9112-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)