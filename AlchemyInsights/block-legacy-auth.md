---
title: BlockLegacyAuth
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
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820198"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="f33ee-102">Eski kimlik doğrulamasını engelleme</span><span class="sxs-lookup"><span data-stu-id="f33ee-102">Blocking legacy authentication</span></span>

<span data-ttu-id="f33ee-103">Eski kimlik doğrulaması, şunların yaptığı kimlik doğrulama isteğine başvuran bir terimdir:</span><span class="sxs-lookup"><span data-stu-id="f33ee-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="f33ee-104">Modern kimlik doğrulaması kullanmayan eski Office istemcileri (örneğin, Office 2010 istemcisi).</span><span class="sxs-lookup"><span data-stu-id="f33ee-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="f33ee-105">IMAP/SMTP/POP3 gibi eski posta protokolleri kullanan tüm istemciler.</span><span class="sxs-lookup"><span data-stu-id="f33ee-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="f33ee-106">Eski kimlik doğrulamasını engelleme ve modern kimlik doğrulamayı etkinleştirme hakkında daha fazla bilgi için Eski kimlik [doğrulamasını engelleme 'ye bakın.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="f33ee-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="f33ee-107">Azure Active Directory'de (Azure AD) güvenlik varsayılanları, güvenliğin daha kolay hale geliyor ve kuruma korumada yardımcı oluyor.</span><span class="sxs-lookup"><span data-stu-id="f33ee-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="f33ee-108">Güvenlik varsayılanları, yaygın saldırılar için önceden yapılandırılmış güvenlik ayarları içerir.</span><span class="sxs-lookup"><span data-stu-id="f33ee-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="f33ee-109">Güvenlik varsayılanları hakkında daha fazla bilgi için [bkz. Güvenlik varsayılanları nedir?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="f33ee-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="f33ee-110">**Not:** Kiracınız 22 Ekim 2019'da veya daha sonra oluşturuldu ise, yeni varsayılan güvenli davranışı yaşıyor ve kiracıda zaten güvenlik varsayılanlarını etkinleştirmişsiniz olabilir.</span><span class="sxs-lookup"><span data-stu-id="f33ee-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="f33ee-111">Kullanıcılarımızın hepsini korumak için, güvenlik varsayılanları oluşturulan tüm yeni kiracılara yuvarlanıyor.</span><span class="sxs-lookup"><span data-stu-id="f33ee-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
