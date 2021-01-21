---
title: Belirteç ömürleri yapılandırma ve genişletme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917199"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="664c4-102">Belirteç ömürleri yapılandırma ve genişletme</span><span class="sxs-lookup"><span data-stu-id="664c4-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="664c4-103">Microsoft Identity platform tarafından verilen bir Access, SAML veya KIMLIK belirtecinin ömrünü belirtebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="664c4-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="664c4-104">Kuruluşunuzdaki tüm uygulamalar için, birden çok kiracı (çok kuruluş) uygulaması veya kuruluşunuzdaki belirli bir hizmet sorumlusu için belirteç ömürleri ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="664c4-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="664c4-105">Daha fazla bilgi için [yapılandırılabilir belirteç ömürleri](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)makalesini okuyun.</span><span class="sxs-lookup"><span data-stu-id="664c4-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="664c4-106">Örnekler için, [belirteç ömürleri yapılandırma ile ilgili örnekleri](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)okuyun.</span><span class="sxs-lookup"><span data-stu-id="664c4-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="664c4-107">Azure Active Directory B2C 'de bir simgenin kullanım ömrünü ve uyumluluğunu nasıl yapılandıracağınızı öğrenmek için, [Azure Active DIRECTORY B2C 'de belirteçleri yapılandırma](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="664c4-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="664c4-108">[Azure Active Directory 'de oturum davranışını yapılandırma](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) : Azure AD B2C 'de kullanılan çoklu oturum açma (SSO) yöntemlerini açıklar ve ilkenizi yapılandırırken en uygun SSO yöntemini seçmenize yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="664c4-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="664c4-109">**Ne kadar çok simge kullanıyorsunuz? Ne kadar sürer?**</span><span class="sxs-lookup"><span data-stu-id="664c4-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="664c4-110">Belirteç ömürleri 1 saat ve oturum yaşam süresi 24 saattir.</span><span class="sxs-lookup"><span data-stu-id="664c4-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="664c4-111">Bu, 24 saat içinde hiçbir istekte bulunulmadığı durumlarda, yeni bir belirteç istemeden önce yeniden oturum açmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="664c4-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="664c4-112">30 Mayıs 2020 ' den sonra, oturum ve yenileme belirteçlerini yapılandırma</span><span class="sxs-lookup"><span data-stu-id="664c4-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="664c4-113">Kullanımdan kalkma, var olan oturum ve yenileme belirteçleri ilkeleriyle bu kadar çok ay içinde gerçekleşecektir.</span><span class="sxs-lookup"><span data-stu-id="664c4-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="664c4-114">Yine de erişim belirteci ömürleri 'ni kullanımdan kaldırma.</span><span class="sxs-lookup"><span data-stu-id="664c4-114">You can still configure access token lifetimes after the deprecation.</span></span>






