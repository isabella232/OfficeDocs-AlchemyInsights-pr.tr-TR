---
title: Parola ilkeleri
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747056"
---
# <a name="password-policies"></a><span data-ttu-id="c1751-102">Parola ilkeleri</span><span class="sxs-lookup"><span data-stu-id="c1751-102">Password policies</span></span>

<span data-ttu-id="c1751-103">**Kullanıcının parola ilkesiyle ilgili sorunlar var**</span><span class="sxs-lookup"><span data-stu-id="c1751-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="c1751-104">Kullanıcının parola ilkesi, kullanıcının yalnızca bulut mu yoksa şirket içi mi olduğuna bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="c1751-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="c1751-105">Yalnızca bulut kullanıcılarının bu makaledeki gereksinimleri karşılayacak bir parola seçmesi gerekir: Yalnızca bulut kullanıcı [hesaplarına](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts) uygulanacak parola ilkeleri</span><span class="sxs-lookup"><span data-stu-id="c1751-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="c1751-106">Şirket içi kullanıcıların şirket içi gereksinimlerini karşılayacak bir parola seçmeleri gerekir.</span><span class="sxs-lookup"><span data-stu-id="c1751-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="c1751-107">Şirket içi kullanıcı parolasını ayarlamıyorsa, şirket içi gereksinimlerinizi kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="c1751-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="c1751-108">**Parola süre sonu ilkelerini ayarlamayı veya denetlemeyi bilmiyorum**</span><span class="sxs-lookup"><span data-stu-id="c1751-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="c1751-109">PowerShell kullanarak kiracıdaki bulut kullanıcıları için süre sonu ilkesi ayarp denetlemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="c1751-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="c1751-110">Bu makaledeki yönergeleri izleyin: [PowerShell kullanarak parola ilkelerini ayarlama veya denetleme](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="c1751-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="c1751-111">Şirket içi kullanıcıların parola süre sonu ilkesi şirket içi AD'nize ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="c1751-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="c1751-112">**Diğer Yararlı bağlantılar:**</span><span class="sxs-lookup"><span data-stu-id="c1751-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="c1751-113">Parola Sıfırlama ile Çalışmaya Başlama</span><span class="sxs-lookup"><span data-stu-id="c1751-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="c1751-114">Yönetici tarafından başlatılan Parola Sıfırlama sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="c1751-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
