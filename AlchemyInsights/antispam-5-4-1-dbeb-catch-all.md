---
title: AntiSpam 5.4.1 VSEÇŞB yakala-tümü
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717381"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="30c82-102">Hata kodu 550 5.4.1 geçiş erişimi reddedildi için teslim sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="30c82-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="30c82-103">Bu sorun, Microsoft ağını girerken geri [sıçramasını önleyen bir e-posta adresinin geçerli olup olmadığını denetlemek için](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) görülür.</span><span class="sxs-lookup"><span data-stu-id="30c82-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="30c82-104">Aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="30c82-104">Try the following:</span></span>

1. <span data-ttu-id="30c82-105">Sorunun tüm etki alanına mı yoksa tek bir e-posta adresine mi özgü olduğunu belirleme:</span><span class="sxs-lookup"><span data-stu-id="30c82-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="30c82-106">Tüm etki alanı: bazen etki alanının eşitlenmesi gereklidir; [etki alanını iç öğesine ayarlamayı ve ardından yetkilendirmeli 'a geri dönün](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="30c82-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="30c82-107">Tek e-posta adresi: bazen adresin eşitlenmesi gereklidir; SMTP proxy adresini değiştirip geri değiştirmek yardım edebilir.</span><span class="sxs-lookup"><span data-stu-id="30c82-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="30c82-108">Sorunun bir gruba veya ortak klasöre özgü olup olmadığını belirleme.</span><span class="sxs-lookup"><span data-stu-id="30c82-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="30c82-109">Bazı nesne türlerinde, nesnelerin Azure Active Directory 'de el ile oluşturulması gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="30c82-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="30c82-110">Ek yardıma ihtiyacınız varsa, lütfen bir destek bileti açın ve sorunun kapsamını (göndermekte olduğunuz nesnenin türü de dahil olmak üzere) belirtin, böylece daha iyi yardımcı olabiliriz.</span><span class="sxs-lookup"><span data-stu-id="30c82-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>