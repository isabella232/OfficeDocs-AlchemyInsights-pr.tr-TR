---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821467"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="f2265-102">Hata kodu 550 5.4.1 Geçiş Erişimi Reddedildi hata kodu için teslim sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="f2265-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="f2265-103">Microsoft ağına girerken [geri dönüşleri önlemek için bir e-posta](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) adresinin geçerli olup olmadığını kontrol etmek bu soruna neden olur.</span><span class="sxs-lookup"><span data-stu-id="f2265-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="f2265-104">Şunları deneyin:</span><span class="sxs-lookup"><span data-stu-id="f2265-104">Try the following:</span></span>

1. <span data-ttu-id="f2265-105">Sorunun bir etki alanının tamamına mı yoksa tek bir e-posta adresine mi özgü olduğunu belirleme:</span><span class="sxs-lookup"><span data-stu-id="f2265-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="f2265-106">Tüm etki alanı: Bazen etki alanının eşitlenmesi gerekir; etki [alanını İç olarak ayarlamayı deneyin ve sonra Yetkili ayarına geri dönebilirsiniz.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="f2265-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="f2265-107">Tek e-posta adresi: Bazen adresin eşitlenmesi gerekir; smtp ara sunucu adresini değiştirmek ve sonra yeniden değiştirmek yardımcı olabilir.</span><span class="sxs-lookup"><span data-stu-id="f2265-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="f2265-108">Sorunun bir gruba mı yoksa ortak klasöre mi özel olduğunu belirler.</span><span class="sxs-lookup"><span data-stu-id="f2265-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="f2265-109">Bazı nesne türlerinde, nesnelerin Azure Active Directory'de el ile oluşturulmuş olması gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="f2265-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="f2265-110">Daha fazla yardım gerekirse, lütfen bir destek bileti açın ve size daha iyi yardımcı olmak için sorunun kapsamını (gönderirken hangi tür nesne dahil) belirtin.</span><span class="sxs-lookup"><span data-stu-id="f2265-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>