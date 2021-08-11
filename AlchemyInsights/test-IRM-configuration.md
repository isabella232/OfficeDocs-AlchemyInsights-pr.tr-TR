---
title: Yeni OME özellikleri için IRM Yapılandırmasını Test
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812449"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Yeni OME özellikleri için IRM Yapılandırmasını Test

Microsoft 365 kiracının yeni OME özelliklerini kullanmak üzere yapılandırılmış olduğunu doğrulamak için, Exchange Online PowerShell'e bağlıyken aşağıdaki [cmdlet'leri çalıştırın:](/powershell/exchange/exchange-online-powershell)


1. çalıştırarak kiracının IRM yapılandırmasını kontrol `Get-IRMConfiguration` edin. Bu değerlerin Doğru olarak ayar olduğundan emin **olun:**
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Etki alanınızı, gönderen adresinizi ve alıcınızı kullanarak `Test-IRMConfiguration` çalıştırın. Sınama başarılı olursa, IRM yapılandırmanızı araştıryın.

IRM yapılandırmasını doğrulama hakkında daha fazla bilgi için bkz. [Exchange Online PowerShell'de yeni OME yapılandırmasını doğrulama.](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)