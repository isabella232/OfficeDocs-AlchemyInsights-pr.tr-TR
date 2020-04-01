---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: e7bff5f9fcf6f2f2c77e93c2f27f585f2cc18bea
ms.sourcegitcommit: 98231a228ecb2bf14ec3b96d4dd4ccf2507617a3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/01/2020
ms.locfileid: "43079280"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="bf10d-102">Eski kimlik doğrulamayı engelleme</span><span class="sxs-lookup"><span data-stu-id="bf10d-102">Blocking legacy authentication</span></span>

<span data-ttu-id="bf10d-103">Eski kimlik doğrulaması, şu lar tarafından yapılan bir kimlik doğrulama isteğini ifade eden bir terimdir:</span><span class="sxs-lookup"><span data-stu-id="bf10d-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="bf10d-104">Modern kimlik doğrulaması kullanmayan eski Office istemcileri (örneğin, Office 2010 istemcisi).</span><span class="sxs-lookup"><span data-stu-id="bf10d-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="bf10d-105">IMAP/SMTP/POP3 gibi eski posta protokollerini kullanan tüm istemciler.</span><span class="sxs-lookup"><span data-stu-id="bf10d-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="bf10d-106">Eski kimlik doğrulamasını engelleme ve modern kimlik doğrulamayı etkinleştirme hakkında daha fazla bilgi için eski [kimlik doğrulamasını engelleme'ye](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)bakın.</span><span class="sxs-lookup"><span data-stu-id="bf10d-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="bf10d-107">Azure Etkin Dizini'ndeki (Azure AD) güvenlik varsayılanları, güvenli olmayı kolaylaştırır ve kuruluşunuzun korunmasına yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="bf10d-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="bf10d-108">Güvenlik varsayılanları, sık yapılan saldırılar için önceden yapılandırılmış güvenlik ayarları içerir.</span><span class="sxs-lookup"><span data-stu-id="bf10d-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="bf10d-109">Güvenlik varsayılanları hakkında daha fazla bilgi [için, güvenlik varsayılanları nelerdir?'](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="bf10d-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="bf10d-110">**Not**: Kiracınız 22 Ekim 2019 tarihinde veya sonrasında oluşturulduysa, yeni güvenli ve varsayılan davranışı yaşıyor olabilirsiniz ve kiracınızda zaten güvenlik varsayılanları etkinleştirilmiştir.</span><span class="sxs-lookup"><span data-stu-id="bf10d-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="bf10d-111">Tüm kullanıcılarımızı korumak amacıyla, güvenlik varsayılanları oluşturulan tüm yeni kiracılara dağıtılıyor.</span><span class="sxs-lookup"><span data-stu-id="bf10d-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
