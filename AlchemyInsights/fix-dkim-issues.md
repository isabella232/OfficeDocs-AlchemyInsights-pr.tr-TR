---
title: DKIM kurulum sorunlarını düzeltme
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506794"
---
# <a name="fix-dkim-setup-issues"></a>DKIM kurulum sorunlarını düzeltme

Özel etki alanınız için DKIM'i etkinleştiren sorunlarla karşılaşırsanız, aşağıdaki adımları kullanın:

- Çoğu DKIM kurulum sorunları yanlış DNS kayıtlarıyla ilişkilidir. DKIM CNAME kaydının (TXT kaydı**değil)** doğru biçimlendirilmiş olduğunu doğrulayın. Daha fazla bilgi için bu [konuya](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)bakın.

- Etki alanınız için DNS barındırma hizmetinde DKIM DNS kayıtlarınızı oluşturduktan veya güncelledikten sonra (genellikle etki alanı kayıt şirketiniz), DNS kayıtlarının yayılmasını bekleyin.

- Yönetici merkezinde DKIM DNS kayıtlarını oluşturamıyorsanız, \<CustomDomain\> özel etki alanınızın (örneğin, contoso.com) değiştirip bu komutu [Exchange Online PowerShell'de](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)çalıştırabilirsiniz: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
