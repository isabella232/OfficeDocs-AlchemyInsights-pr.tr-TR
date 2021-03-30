---
title: API İzinleri ve İzin Süreci
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
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405444"
---
# <a name="api-permissions-and-consent-process"></a>API İzinleri ve İzin Süreci

Uygulamanın Microsoft Graph'te verilere erişmesi için, kullanıcı veya yöneticinin izin süreci aracılığıyla ona doğru izinleri ataması gerekir. [Microsoft Graph izinleri başvurusu,](https://docs.microsoft.com/graph/permissions-reference) her büyük Microsoft Graph API kümesiyle ilişkilendirilmiş izinleri listeler. Ayrıca, izinleri kullanma konusunda da yol göstermeyi sağlar.

**Hizmet sorumlusu ayarlama veya güncelleştirme**

- [Serviceprincipal oluşturma](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - Bu makalede, yeni servicePrincipal nesnesinin nasıl oluşturularak oluşturulacı yermektedir.
- [Portalda Azure AD uygulaması &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) hizmet sorumlusu oluşturma - Bu makalede, rol tabanlı erişim denetimiyle birlikte 2013'te 2013'te 2013'te 2013'te 2013'te 2013'te 2013'e kadar olan yeni bir Azure Active Directory (Azure AD) uygulaması ve hizmet sorumlusu nasıl oluşturulmaktadır?
- [Uygulamalar& Azure AD'de](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) hizmet sorumlularını içerir - Bu makalede, Azure Active Directory'de uygulama kaydı, uygulama nesneleri ve hizmet sorumluları açıklanmıştır: bunların ne olduğu, bunların nasıl kullanıldıkları ve birbirlerine nasıl bağlı olduğu.

**Uygulama kaydını ekleme veya güncelleştirme ve yönetici iznini sağlama**

- [Uygulama kaydı oluşturma](https://docs.microsoft.com/graph/api/application-post-applications) - Bu makalede, yeni bir uygulama nesnesinin nasıl oluşturularak oluşturul açıklanmıştır.
- [Uygulama kaydını güncelleştirme - API izinleri](https://docs.microsoft.com/graph/api/application-update) - Bu makalede, uygulama nesnesinin özelliklerini nasıl güncelleştirebilirsiniz?
- [Yönetici onayı sağlama](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - Genel olarak yönetici onayı ve onayı için, yöneticinin açıkça izinler sağlamasını gerektiririz.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Tek bir rol atamasında birden çok anaparayı ve birden çok kapsamı destekleyen Microsoft 365 RBAC sağlayıcıları için birleşik rol tanımları ve rol atamaları için rol yönetim kapsayıcısı. Bu, *rbacApplication kaynak türünden* farklıdır. Microsoft Intune, bu tür bir RBAC sağlayıcısı örneğidir. Intune'daki bir rol atamasında bir sorumlular dizisi ve bir kapsam grupları dizisi olabilir. **Bu betadır; yani hala geliştirme aşamasındadır ve üretimde kullanılması önerilmez.**
