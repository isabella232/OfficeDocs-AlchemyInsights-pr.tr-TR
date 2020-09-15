---
title: BlockLegacyAuth
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
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685618"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="a9e73-102">Eski kimlik doğrulama engelleniyor</span><span class="sxs-lookup"><span data-stu-id="a9e73-102">Blocking legacy authentication</span></span>

<span data-ttu-id="a9e73-103">Eski kimlik doğrulama, bir kimlik doğrulama isteğine başvuran bir terimdir:</span><span class="sxs-lookup"><span data-stu-id="a9e73-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="a9e73-104">Modern kimlik doğrulama kullanmayan eski Office istemcileri (örneğin, Office 2010 istemcisi).</span><span class="sxs-lookup"><span data-stu-id="a9e73-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="a9e73-105">IMAP/SMTP/POP3 gibi eski posta protokollerini kullanan tüm istemciler.</span><span class="sxs-lookup"><span data-stu-id="a9e73-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="a9e73-106">Eski kimlik doğrulamayı engelleme ve modern kimlik doğrulamayı etkinleştirme hakkında daha fazla bilgi için, [eski kimlik doğrulamasını engellemeye](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)bakın.</span><span class="sxs-lookup"><span data-stu-id="a9e73-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="a9e73-107">Azure Active Directory 'deki güvenlik Varsayılanları (Azure AD) güvenli olmasını ve kuruluşunuzun korunmasına yardımcı olmasını kolaylaştırır.</span><span class="sxs-lookup"><span data-stu-id="a9e73-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="a9e73-108">Güvenlik Varsayılanları, yaygın saldırılar için önceden yapılandırılmış güvenlik ayarlarını içerir.</span><span class="sxs-lookup"><span data-stu-id="a9e73-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="a9e73-109">Güvenlik Varsayılanları hakkında daha fazla bilgi için [güvenlik Varsayılanları nelerdir?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="a9e73-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="a9e73-110">**Not**: kiracınız 22nd, 2019 tarihinde veya bu tarihten sonra oluşturulduysa, yeni güvenli-varsayılan davranışla karşılaşmanız ve zaten kiracınızda güvenlik Varsayılanları etkinleştirilmiş olabilir.</span><span class="sxs-lookup"><span data-stu-id="a9e73-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="a9e73-111">Tüm kullanıcılarımızı koruduğumuz bir çabayla, güvenlik Varsayılanları oluşturulan tüm yeni kiracıları alır.</span><span class="sxs-lookup"><span data-stu-id="a9e73-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
