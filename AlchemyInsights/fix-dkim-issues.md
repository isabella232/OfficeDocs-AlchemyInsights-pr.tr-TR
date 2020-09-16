---
title: Bu kurulum sorunlarını düzeltin
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
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744970"
---
# <a name="fix-dkim-setup-issues"></a>Bu kurulum sorunlarını düzeltin

Özel etki alanınız için bazı sorunları etkinleştirmekle karşılaşırsanız aşağıdaki adımları kullanın:

- Çoğu VSEÇKIM kurulum sorunları, hatalı DNS kayıtlarıyla ilgilidir. VSEÇKIM CNAME kaydının (TXT kaydı**değil** ) doğru biçimlendirildiğini doğrulayın. Daha fazla bilgi için bu [konuya](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)bakın.

- Etki alanınız için DNS barındırma hizmetine yönelik DNS kayıtlarınızı oluşturduktan veya güncelleştirdikten sonra (genellikle etki alanı kayıt şirketiniz), DNS kayıtlarının yayılmasına kadar bekleyin.

- Yönetim merkezinde DNS kayıtlarını oluşturamadığınızda, \<CustomDomain\> özel etki alanınızla (örneğin, contoso.com) değiştirebilirsiniz ve bu komutu [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)'de çalıştırabilirsiniz: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
