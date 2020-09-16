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
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="76f18-102">Bu kurulum sorunlarını düzeltin</span><span class="sxs-lookup"><span data-stu-id="76f18-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="76f18-103">Özel etki alanınız için bazı sorunları etkinleştirmekle karşılaşırsanız aşağıdaki adımları kullanın:</span><span class="sxs-lookup"><span data-stu-id="76f18-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="76f18-104">Çoğu VSEÇKIM kurulum sorunları, hatalı DNS kayıtlarıyla ilgilidir.</span><span class="sxs-lookup"><span data-stu-id="76f18-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="76f18-105">VSEÇKIM CNAME kaydının (TXT kaydı**değil** ) doğru biçimlendirildiğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="76f18-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="76f18-106">Daha fazla bilgi için bu [konuya](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)bakın.</span><span class="sxs-lookup"><span data-stu-id="76f18-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="76f18-107">Etki alanınız için DNS barındırma hizmetine yönelik DNS kayıtlarınızı oluşturduktan veya güncelleştirdikten sonra (genellikle etki alanı kayıt şirketiniz), DNS kayıtlarının yayılmasına kadar bekleyin.</span><span class="sxs-lookup"><span data-stu-id="76f18-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="76f18-108">Yönetim merkezinde DNS kayıtlarını oluşturamadığınızda, \<CustomDomain\> özel etki alanınızla (örneğin, contoso.com) değiştirebilirsiniz ve bu komutu [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)'de çalıştırabilirsiniz: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="76f18-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
