---
title: Kullanıcı onayı sorunlarını giderme
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901626"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="0bf7f-102">Kullanıcı onayı sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="0bf7f-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="0bf7f-103">Son kullanıcıların Azure portalı veya PowerShell aracılığıyla uygulamalara nasıl izin vermiş olduğunu yapılandırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0bf7f-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="0bf7f-104">Daha fazla bilgi için [Kullanıcı onayı ayarlarına](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) bakın.</span><span class="sxs-lookup"><span data-stu-id="0bf7f-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="0bf7f-105">Yönetici, tek bir kullanıcı adına temsilci izinlerine izin vermek için [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) 'yi de kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="0bf7f-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="0bf7f-106">Daha fazla bilgi için, [Kullanıcı adına erişim alma](https://docs.microsoft.com/graph/auth-v2-user)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="0bf7f-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="0bf7f-107">[Kullanıcı onayı hataları](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): Bu makalede, bir uygulamaya uyum sürecinde oluşabilecek hatalar açıklanır.</span><span class="sxs-lookup"><span data-stu-id="0bf7f-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="0bf7f-108">Herhangi bir hata iletisi içermeyen beklenmeyen onay istemleriyle ilgili sorun yaşıyorsanız, [Azure AD Için kimlik doğrulama senaryolarını](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)inceleyin.</span><span class="sxs-lookup"><span data-stu-id="0bf7f-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>