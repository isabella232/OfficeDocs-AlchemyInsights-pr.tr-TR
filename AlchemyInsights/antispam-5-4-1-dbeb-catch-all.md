---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707931"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="8e6d5-102">Hata kodu 550 5.4.1 Röle Erişimi Reddedildi için teslim sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="8e6d5-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="8e6d5-103">Bu sorun, Microsoft ağına girerken [geri dönüşleri önlemek için bir e-posta adresinin geçerli olup olmadığını kontrol](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ederken oluşur.</span><span class="sxs-lookup"><span data-stu-id="8e6d5-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="8e6d5-104">Aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="8e6d5-104">Try the following:</span></span>

1. <span data-ttu-id="8e6d5-105">Sorunun tüm etki alanına mı yoksa tek bir e-posta adresine mi özgü olduğunu belirleyin:</span><span class="sxs-lookup"><span data-stu-id="8e6d5-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="8e6d5-106">Tüm etki alanı: Bazen etki alanının eşitlemesi gerekir; [etki alanını İçe ayarlamayı deneyin ve ardından Yetkili'ye geri dönmeyi](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)deneyin.</span><span class="sxs-lookup"><span data-stu-id="8e6d5-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="8e6d5-107">Tek e-posta adresi: Bazen adresin senkronize edilmesi gerekir; smtp proxy adresini değiştirmek ve sonra geri değiştirme yardımcı olabilir.</span><span class="sxs-lookup"><span data-stu-id="8e6d5-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="8e6d5-108">Sorunun bir gruba mı yoksa ortak klasöre mi özgü olduğunu belirleyin.</span><span class="sxs-lookup"><span data-stu-id="8e6d5-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="8e6d5-109">Bazı nesne türleri için nesnelerin Azure Etkin Dizini'nde el ile oluşturulması gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="8e6d5-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="8e6d5-110">Ek yardıma ihtiyacınız varsa, size daha iyi yardımcı olmamız için lütfen bir destek bileti açın ve sorunun kapsamını (gönderdiğiniz nesnenin türü dahil) belirtin.</span><span class="sxs-lookup"><span data-stu-id="8e6d5-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>