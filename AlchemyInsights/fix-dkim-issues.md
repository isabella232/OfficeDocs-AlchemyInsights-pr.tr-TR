---
title: DKIM kurulum sorunlarını düzeltme
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945951"
---
# <a name="fix-dkim-setup-issues"></a>DKIM kurulum sorunlarını düzeltme

Özel etki alanınız için DKIM'i etkinleştirme sorunlarıyla karşılaşılan bir sorun varsa, aşağıdaki adımları kullanın:

- DKIM kurulum sorunlarının çoğu hatalı DNS kayıtlarıyla ilgili. DKIM CNAME kaydının (TXT **kaydı** değil) doğru biçimlendiril olduğunu doğrulayın. Daha fazla bilgi için bu konuya [bakın.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- Etki alanınız için DNS barındırma hizmette DKIM DNS kayıtlarınızı oluşturduktan veya güncelleştirdikten sonra (normalde, etki alanı kayıt şirketiniz), DNS kayıtlarının yayılmasını bekleyin.

- Yönetim merkezinde DKIM DNS kayıtlarını oluşturasanız bile, özel etki \<CustomDomain\> alanınız ile değiştirebilir (örneğin, contoso.com) ve şu komutu [Exchange Online PowerShell'de çalıştırabilirsiniz:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
