---
title: DKIM kurulum sorunlarını düzeltme
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765505"
---
# <a name="fix-dkim-setup-issues"></a>DKIM kurulum sorunlarını düzeltme

DKIM özel etki alanınız için etkinleştirme sorunlarla karşılaşırsanız, aşağıdaki adımları kullanın:

- Çoğu DKIM kurulum sorunlarını hatalı DNS kayıtlarıyla ilgili. (**Değil** bir TXT kaydı) DKIM CNAME kaydını doğru şekilde biçimlendirilmiş olduğunu doğrulayın. Bu [konuda](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)daha fazla bilgi için bkz.

- Sonra oluşturduğunuz veya DKIM DNS kayıtlarınızı etki alanınızın (tipik olarak, etki alanı Kaydedicisi) hizmetini barındıran DNS güncelleştirme, DNS kayıtlarını yaymak bekleyin.

- DKIM DNS kayıtları Yönetim Merkezi'nde oluşturamazsanız, değiştirebileceğiniz \<CustomDomain\> özel etki alanı (örneğin, contoso.com) ve [Çevrimiçi Exchange PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)içinde bu komutu çalıştırın: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
