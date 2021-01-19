---
title: Oturumu kapatma sorunları
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7793"
- "9004355"
ms.openlocfilehash: 794e5c43340ba4b5c653eda4c11b4480cd3fa710
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901298"
---
# <a name="sign-out-issues"></a><span data-ttu-id="13edf-102">Oturumu kapatma sorunları</span><span class="sxs-lookup"><span data-stu-id="13edf-102">Sign-out issues</span></span>

<span data-ttu-id="13edf-103">Oturumu kapatma ile ilgili sorunları çözmek için aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="13edf-103">To resolve issues related to signing out, perform the following steps:</span></span>

1. <span data-ttu-id="13edf-104">Siz veya bir kullanıcı uygulamaları günlüğe alıyor veya bir Kullanıcı uygulamayı alıyorsa, [Microsoft Identity platformunda koşullu erişim veya yapılandırılabilir belirteç ömürleri](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) [ile kimlik doğrulama oturumu yönetimini yapılandırma](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) makalelerini uygulayın.</span><span class="sxs-lookup"><span data-stu-id="13edf-104">If you or a user are getting logged or kicked out of applications, follow the guidance in the articles [Configure authentication session management with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) or [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
2. <span data-ttu-id="13edf-105">Tüm diğer oturum kapatma hataları veya sorunları, Azure Active Directory 'nin (Azure AD) belirli bir uygulamayla tümleştirilmesine sorun giderirken çözülebilir.</span><span class="sxs-lookup"><span data-stu-id="13edf-105">Most other sign-out errors or problems can be solved by troubleshooting the integration of Azure Active Directory (Azure AD) with the specific application.</span></span> <span data-ttu-id="13edf-106">[Uygulamaları Azure Active Directory ile tümleştirmek için aşağıdaki öğretici topluluğuna](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)giderek belirli bir tümleştirmenin kılavuzunu bulabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="13edf-106">You can find guidance for a specific integration by going to this [collection of tutorials for integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), including:</span></span>
    - <span data-ttu-id="13edf-107">SaaS uygulaması öğreticileri</span><span class="sxs-lookup"><span data-stu-id="13edf-107">SaaS application tutorials</span></span>
    - <span data-ttu-id="13edf-108">Çoklu oturum açma eğitmenleri</span><span class="sxs-lookup"><span data-stu-id="13edf-108">Single sign-on tutorials</span></span>
    - <span data-ttu-id="13edf-109">Kullanıcı tarafından sağlanan öğreticiler</span><span class="sxs-lookup"><span data-stu-id="13edf-109">User-provisioning tutorials</span></span>