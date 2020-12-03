---
title: Kiracı silme
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564877"
---
# <a name="delete-tenant"></a>Kiracı silme

Bir Azure AD silmek için:
- Dizinde genel yöneticisiniz.
- Contoso.onmicrosoft.com gibi varsayılan dizine sahip olan ve admin@contoso.onmicrosoft.com gibi bir hesap ile oturum açmadınız.
- Silmeden önce dizindeki tüm etkin uygulamaları kaldırın. Etkin uygulamaları kaldırmak için uygulama kayıtları 'na gidin ve var olan uygulamaları kaldırın.
- Microsoft Azure, Office 365 veya dizinde ilişkilendirilmiş Azure AD Premium gibi herhangi bir Microsoft Online hizmeti için etkin abonelik yoktur. Azure desteği ve faturalamayla aboneliklerinizi aktarın veya etkin aboneliklerin iptalini yeniden yapın. Office 365 ve Azure aboneliklerini Iptal etme hakkında daha fazla bilgi edinin. Bir kiracıya varolan aboneliği ilişkilendirme veya ekleme konusunda rehberlik için [Azure AD kiracınıza Azure aboneliği ilişkilendirme veya ekleme](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)konusuna bakın.
- Etkin lisans yok. Lisansları kaldırmak için, [lisansı kaldırma aboneliğini](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)kaldırma konusuna bakın.
- Azure AD 'yi silmeye çalışırken, genel yönetici olarak, dizinde başka etkin kullanıcı yok. Tüm etkin kullanıcıları kaldırın ve Kiracıdaki özel bir etki alanı adındaki tüm bağımlılıklar, admin@contoso.com ile oluşturulan kullanıcılar gibi de kaldırılmalıdır.

Bu konuda daha fazla ayrıntı için:
- Azure Active [Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)'yi silme konusuna bakın.
- Dizindeki [uygulamaları kaldırmak, bkz.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
