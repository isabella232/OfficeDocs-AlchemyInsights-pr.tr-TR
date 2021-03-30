---
title: Uygulama Kayıt istemcisinin sırrı veya Sertifika sorunları
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405329"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="74a5f-102">Uygulama Kayıt istemcisinin sırrı veya Sertifika sorunları</span><span class="sxs-lookup"><span data-stu-id="74a5f-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="74a5f-103">Uygulama istemcisinin süresi dolsun mu?</span><span class="sxs-lookup"><span data-stu-id="74a5f-103">Application client secret expiring?</span></span>

<span data-ttu-id="74a5f-104">Kayıtlı uygulamanın nasıl oluşturulduktan bağımsız olarak, uygulamalar Kayıt portalında standart kayıt işlemi aracılığıyla veya Kiracınıza uygulama izni kullanılarak Hizmet Sorumlusu oluşturulmuşsa, geçerli uygulama kodunun sona ermeden önce yeni bir İstemci Sırrı oluşturularak ilgili uygulama kodunda güncelleştirilmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="74a5f-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="74a5f-105">En uzun geçerlilik süresi 2 yıldır.</span><span class="sxs-lookup"><span data-stu-id="74a5f-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="74a5f-106">Bir anımsatıcı olarak gizli değerin, portalda Uygulama kayıtları sayfasından ayrılarak görünmeyebilecek olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="74a5f-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="74a5f-107">Daha fazla bilgi için [bkz. Hızlı Başlangıç: Microsoft](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) kimlik platformuna uygulama kaydetme ve Microsoft kimlik platformu [için en iyi yöntemler.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="74a5f-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="74a5f-108">Daha fazla bilgi edinmek için [portalda Azure AD & hizmet sorumlusu oluşturma - Microsoft kimlik platformuna bakın.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="74a5f-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
