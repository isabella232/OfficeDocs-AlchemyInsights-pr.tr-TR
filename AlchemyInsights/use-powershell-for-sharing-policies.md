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
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Paylaşım ilkeleri ve Organizasyon İlişkileri için Windows PowerShell'i kullanma


Organizasyon ilişkileri için lütfen ayrıntılı söz dizimini ve aşağıdakiler için parametre bilgilerini inceleyin: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  VE  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Paylaşım ilkesi oluşturmak için [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy)'ı kullanın. [Bir posta kutusuna veya kullanıcıya paylaşım ilkesi uygulamak](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) için yeni oluşturulan ilke ile [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) ve [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) birleşimini kullanın. [Bir paylaşım ilkesini düzenlemek, devre dışı bırakmak veya kaldırmak için](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ve [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)'ı kullanmanız gerekiyor.

**Bu konuyu tam olarak anlamak için lütfen aşağıdakini okuyun:**

[Exchange Online'da paylaşım](https://docs.microsoft.com/exchange/sharing/sharing)