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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717582"
---
# <a name="fix-dkim-setup-issues"></a>DKIM kurulum sorunlarını düzeltme

Özel etki alanınız için DKIM'i etkinleştiren sorunlarla karşılaşırsanız, aşağıdaki adımları kullanın:

- Çoğu DKIM kurulum sorunları yanlış DNS kayıtlarıyla ilişkilidir. DKIM CNAME kaydının (TXT kaydı**değil)** doğru biçimlendirilmiş olduğunu doğrulayın. Daha fazla bilgi için bu [konuya](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)bakın.

- Etki alanınız için DNS barındırma hizmetinde DKIM DNS kayıtlarınızı oluşturduktan veya güncelledikten sonra (genellikle etki alanı kayıt şirketiniz), DNS kayıtlarının yayılmasını bekleyin.

- Yönetici \<merkezinde DKIM DNS kayıtlarını oluşturamıyorsanız, CustomDomain'i\> özel etki alanınızın (örneğin, contoso.com) değiştirebilir ve bu komutu Exchange Online [PowerShell'de](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)çalıştırabilirsiniz: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
