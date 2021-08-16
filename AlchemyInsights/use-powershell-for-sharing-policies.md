---
title: Paylaşım ilkeleri ve Organizasyon İlişkileri için Windows PowerShell'i kullanma
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 48df03b1397b0e924aa878cea3d1cac07ca862c3636c1273d10f4841a03fddcf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998516"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Paylaşım ilkeleri ve Organizasyon İlişkileri için Windows PowerShell'i kullanma


Organizasyon ilişkileri için lütfen ayrıntılı söz dizimini ve aşağıdakiler için parametre bilgilerini inceleyin: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  VE  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Paylaşım ilkesi oluşturmak için [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy)'ı kullanın. [Bir posta kutusuna veya kullanıcıya paylaşım ilkesi uygulamak](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) için yeni oluşturulan ilke ile [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) ve [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) birleşimini kullanın. [Bir paylaşım ilkesini düzenlemek, devre dışı bırakmak veya kaldırmak için](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ve [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)'ı kullanmanız gerekiyor.

**Bu konuyu tam olarak anlamak için lütfen aşağıdakini okuyun:**

[Exchange Online'da paylaşım](https://docs.microsoft.com/exchange/sharing/sharing)