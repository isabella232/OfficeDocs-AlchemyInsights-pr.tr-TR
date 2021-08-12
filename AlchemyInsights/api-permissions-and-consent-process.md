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
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932081"
---
# <a name="api-permissions-and-consent-process"></a>API İzinleri ve İzin Süreci

Uygulamanın Microsoft Graph'deki verilere erişmesi için, kullanıcının veya yöneticinin izin süreci aracılığıyla bu verilere doğru izinleri olması gerekir. [Microsoft Graph izinleri başvurusu,](https://docs.microsoft.com/graph/permissions-reference) microsoft veri api'lerinden her bir ana veri kümesiyle Graph listeler. Ayrıca, izinleri kullanma konusunda yol göstermeyi de sağlar.

**Hizmet sorumlularını ayarlama veya güncelleştirme**

- [Serviceprincipal oluşturma](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - Bu makalede, yeni servicePrincipal nesnesinin nasıl oluşturulacı olduğu gösterir.
- [Portalda Bir Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) hizmet sorumlusu oluşturma - Bu makalede, rol tabanlı erişim denetimiyle birlikte kullanılana yeni bir Azure Active Directory (Azure AD) uygulaması ve hizmet sorumlusu oluşturma hakkında bilgi bulabilirsiniz.
- [Uygulamalar & Azure AD'de](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) hizmet sorumlularını içerir - Bu makalede, Azure Active Directory'te uygulama kaydı, uygulama nesneleri ve hizmet sorumluları açıklanmıştır: bunların ne olduğu, nasıl kullanıldıları ve birbirlerine nasıl ilişkilileri.

**Uygulama kaydı ekleme veya güncelleştirme ve yönetici izni sağlama**

- [Uygulama kaydı oluşturma](https://docs.microsoft.com/graph/api/application-post-applications) - Bu makalede yeni bir uygulama nesnesinin nasıl oluşturul olduğu açıklanmıştır.
- [Uygulama kaydını güncelleştirme - API izinleri](https://docs.microsoft.com/graph/api/application-update) - Bu makalede, uygulama nesnesinin özelliklerini nasıl güncelleştirebilirsiniz?
- [Yönetici izni sağlama](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - Genel olarak yöneticinin izni ve onayı için, yöneticinin açıkça izinler gerektirmesi gerekir.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Tek bir rol atamasında birden çok asıl adı ve birden çok kapsamı destekleyen Microsoft 365 RBAC sağlayıcıları için birleşik rol tanımları ve rol atamaları için rol yönetim kapsayıcısı. Bu, *rbacApplication kaynak türünden* farklıdır. Microsoft Intune, böyle bir RBAC sağlayıcısı örneğidir. Intune'daki bir rol atamasında bir dizi sorumlu olabilir ve bir kapsam grubu dizisi olabilir. **Bu beta sürümdedir; başka bir ifadeyle hala geliştirme aşamasındadır ve üretimde kullanılması önerilmez.**
