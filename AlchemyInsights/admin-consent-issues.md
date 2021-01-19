---
title: Yönetici onayı sorunları
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
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901515"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="8308f-102">Yönetici onayı sorunları</span><span class="sxs-lookup"><span data-stu-id="8308f-102">Admin consent issues</span></span>

1. <span data-ttu-id="8308f-103">Kullanıcıların doğrudan onay ekranından yönetici onayı istemesini sağlamak için [yönetici onayı iş akışını](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="8308f-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="8308f-104">Siz veya uygulamanızın kullanıcıları izin işlemi sırasında beklenmeyen hatalar görüyorsanız, sorun giderme adımları için bu makaleye bakın: [bir uygulamaya izin uygularken beklenmeyen hata](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="8308f-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="8308f-105">[Microsoft Identity platformunda yönetici onayı](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)hakkında daha fazla bilgi, [onay isteminin](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) nasıl çalıştığı ve [kiracı genelinde yönetici onayı için bir talebi değerlendirme](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="8308f-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="8308f-106">Microsoft Identity platform ile birleşen uygulamalar, kullanıcıların ve yöneticilerin verilere nasıl erişilebileceğini denetler.</span><span class="sxs-lookup"><span data-stu-id="8308f-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="8308f-107">Yetkilendirme modelinin uygulaması Microsoft Identity platform uç noktasında güncelleştirilmiştir ve bir uygulamanın Microsoft Identity platformuyla etkileşimde bulunma şeklini değiştirir.</span><span class="sxs-lookup"><span data-stu-id="8308f-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="8308f-108">Kapsamlar, izinler ve izin gibi bu yetkilendirme modeline genel bakış için [Microsoft Identity platform uç noktasındaki izinler ve kabul](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) 'e bakın.</span><span class="sxs-lookup"><span data-stu-id="8308f-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>