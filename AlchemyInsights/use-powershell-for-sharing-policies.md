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
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>İlkeleri ve Kuruluş ilişkilerini paylaşmak için PowerShell'i kullanma


Organizasyon ilişkileri için lütfen detaylı sözdizimi ve parametre bilgilerini gözden geçirin: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) AND [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Paylaşım ilkesi oluşturmak için [Yeni Paylaşım Politikası'nı](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy)kullanın. [Bir posta kutusuna veya kullanıcıya paylaşım ilkesi uygulamak için,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) yeni oluşturulan ilkeyle [Set-Posta Kutusu](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) ve [Get-Mailbox'ın](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) birleşimini kullanmanız gerekir. [Bir paylaşım ilkesini değiştirmek, devre dışı kaldırıp kaldırmak](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) için [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ve [Remove-SharingPolicy'yi](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)kullanmanız gerekir.

**Bu konunun tam olarak anlaşılması için lütfen okuyun:**

[Exchange Online'da Paylaşım](https://docs.microsoft.com/exchange/sharing/sharing)