---
title: SSPR sorunlarını giderme
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430361"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="27669-102">SSPR sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="27669-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="27669-103">**Parola sıfırlamayı yapılandırmada sorun istemiyorum**</span><span class="sxs-lookup"><span data-stu-id="27669-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="27669-104">Yöneticiyseniz ve kendi kendine parola sıfırlamayı nasıl etkinleştirebilirsiniz diye arıyorsanız, [öğreticide SSPR'yi](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)etkinleştirme, parola sıfırlamayı yapılandırmaya bakın.</span><span class="sxs-lookup"><span data-stu-id="27669-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="27669-105">Lisans gereksinimlerini gözden geçirmek [de istiyor olabilirsiniz.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="27669-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="27669-106">Kuruluşta en az bir lisans atanmış olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="27669-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="27669-107">**Yalnızca bulut kullanıcıları** - Ücretli tüm Office 365 (O365) SKU'ları veya Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="27669-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="27669-108">**Bulut ve/veya şirket içi** kullanıcılar - Azure AD Premium P1 veya P2, Enterprise Mobility + Security (EMS) veya Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="27669-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="27669-109">Self servis parola sıfırlama hakkında daha fazla soru için SSS [bölümlerimizi inceleyin.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="27669-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="27669-110">**Hata iletisi alıyorum**</span><span class="sxs-lookup"><span data-stu-id="27669-110">**I'm getting an error message**</span></span>

<span data-ttu-id="27669-111">Sık karşılaşılan hataları ve bunların çözümlerini bulmak için bu makaleyi gözden geçirme: Self [servis parola sıfırlama sorunlarını giderme](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="27669-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="27669-112">**Parola sıfırlama ilkemde sorun var**</span><span class="sxs-lookup"><span data-stu-id="27669-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="27669-113">Parola sıfırlama ilkeniz beklendiği gibilenmiyorsa veya parola sıfırlama ilkeleri hakkında sorularınız varsa şu makaleyi gözden geçirebilirsiniz: Azure Active Directory'de parola ilkeleri ve [kısıtlamaları.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="27669-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="27669-114">Parola sıfırlama ilkeleri yöneticiler için geçerli değildir.</span><span class="sxs-lookup"><span data-stu-id="27669-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="27669-115">Microsoft, herhangi bir Azure yönetici rolü için güçlü bir varsayılan iki kapılı parola sıfırlama ilkesi zorunlu tutulmaktadır.</span><span class="sxs-lookup"><span data-stu-id="27669-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="27669-116">Yönetici olmadığınız bir kullanıcıyla test etmekte olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="27669-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="27669-117">Yönetici sıfırlama ilkesi hakkında daha fazla bilgi için bu makaleye bakın: Yönetici sıfırlama [ilkesi farklılıkları.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="27669-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="27669-118">**Kullanıcılarımı parola sıfırlama için ek güvenlik bilgileri kaydetmelerini istemiyorum**</span><span class="sxs-lookup"><span data-stu-id="27669-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="27669-119">API, PowerShell veya Azure AD Connect kullanarak kullanıcılarınız için verileri (e-posta ve telefon öznitelikleri) önceden doldurmak için kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="27669-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="27669-120">Okumayı öğrenmek için:</span><span class="sxs-lookup"><span data-stu-id="27669-120">To learn how read:</span></span>

- [<span data-ttu-id="27669-121">Kullanıcıların kaydolması gerekmeden parola sıfırlamayı dağıtma</span><span class="sxs-lookup"><span data-stu-id="27669-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="27669-122">Parola sıfırlama ile kullanılan veriler</span><span class="sxs-lookup"><span data-stu-id="27669-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="27669-123">**Kullanıcılarımı parola sıfırlama için ek güvenlik bilgilerini kaydetmelerini istiyorum**</span><span class="sxs-lookup"><span data-stu-id="27669-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="27669-124">Kullanıcılarınızı, güvenlik bilgilerini kendi kendine parola sıfırlama için kaydetmelerini ve bu bilgileri kullanıcılarınızı [aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)</span><span class="sxs-lookup"><span data-stu-id="27669-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="27669-125">Veriler kullanıcı (kullanıcı veya yönetici tarafından) doldurulduğunda, kullanıcılarınızı kendi parolalarını [sıfırlama](https://passwordreset.microsoftonline.com/) gücü aka.ms/sspr için kullanıcınızı e-postaya yönlendirin.</span><span class="sxs-lookup"><span data-stu-id="27669-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="27669-126">Kullanıcılar hala sorun yaşıyorsa, bunlar büyük olasılıkla **federasyon** veya parola karması **eşitlenmiş kullanıcılardır.**</span><span class="sxs-lookup"><span data-stu-id="27669-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="27669-127">Bu, Büyük olasılıkla Parola Geri Yazma hizmetiyle ilgili bir sorun olduğu anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="27669-127">This means there is likely a problem with the Password Writeback service.</span></span>