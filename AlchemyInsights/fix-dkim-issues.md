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
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="82337-102">DKIM kurulum sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="82337-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="82337-103">Özel etki alanınız için DKIM'i etkinleştiren sorunlarla karşılaşırsanız, aşağıdaki adımları kullanın:</span><span class="sxs-lookup"><span data-stu-id="82337-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="82337-104">Çoğu DKIM kurulum sorunları yanlış DNS kayıtlarıyla ilişkilidir.</span><span class="sxs-lookup"><span data-stu-id="82337-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="82337-105">DKIM CNAME kaydının (TXT kaydı**değil)** doğru biçimlendirilmiş olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="82337-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="82337-106">Daha fazla bilgi için bu [konuya](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)bakın.</span><span class="sxs-lookup"><span data-stu-id="82337-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="82337-107">Etki alanınız için DNS barındırma hizmetinde DKIM DNS kayıtlarınızı oluşturduktan veya güncelledikten sonra (genellikle etki alanı kayıt şirketiniz), DNS kayıtlarının yayılmasını bekleyin.</span><span class="sxs-lookup"><span data-stu-id="82337-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="82337-108">Yönetici merkezinde DKIM DNS kayıtlarını oluşturamıyorsanız, \<CustomDomain\> özel etki alanınızın (örneğin, contoso.com) değiştirip bu komutu [Exchange Online PowerShell'de](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)çalıştırabilirsiniz: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="82337-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
