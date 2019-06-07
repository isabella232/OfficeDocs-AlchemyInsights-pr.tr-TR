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
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="2d744-102">DKIM kurulum sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="2d744-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="2d744-103">DKIM özel etki alanınız için etkinleştirme sorunlarla karşılaşırsanız, aşağıdaki adımları kullanın:</span><span class="sxs-lookup"><span data-stu-id="2d744-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="2d744-104">Çoğu DKIM kurulum sorunlarını hatalı DNS kayıtlarıyla ilgili.</span><span class="sxs-lookup"><span data-stu-id="2d744-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="2d744-105">(**Değil** bir TXT kaydı) DKIM CNAME kaydını doğru şekilde biçimlendirilmiş olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="2d744-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="2d744-106">Bu [konuda](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="2d744-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="2d744-107">Sonra oluşturduğunuz veya DKIM DNS kayıtlarınızı etki alanınızın (tipik olarak, etki alanı Kaydedicisi) hizmetini barındıran DNS güncelleştirme, DNS kayıtlarını yaymak bekleyin.</span><span class="sxs-lookup"><span data-stu-id="2d744-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="2d744-108">DKIM DNS kayıtları Yönetim Merkezi'nde oluşturamazsanız, değiştirebileceğiniz \<CustomDomain\> özel etki alanı (örneğin, contoso.com) ve [Çevrimiçi Exchange PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)içinde bu komutu çalıştırın: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="2d744-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
