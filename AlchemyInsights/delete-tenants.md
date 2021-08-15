---
title: Kiracıyı silme
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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993913"
---
# <a name="delete-tenant"></a>Kiracıyı silme

Azure AD'den silmek için şunları emin edin:
- Dizinde bir Genel Yöneticisiniz.
- Oturum açık oturum açın hesabıyla, örneğin oturum contoso.onmicrosoft.com varsayılan dizini olan bir hesap ile oturum admin@contoso.onmicrosoft.com.
- Silmeden önce dizinde tüm etkin uygulamaları kaldırın. Etkin uygulamaları kaldırmak için Uygulama kayıtları'ne gidin ve var olan uygulamaları kaldırın.
- Dizinle ilişkilendirilmiş çevrimiçi hizmetler, hizmetler veya Microsoft Azure Office 365 Microsoft Online Services Azure AD Premium abonelik yoktur. Aboneliklerinizi aktarın veya Azure Destek ve Faturalama yoluyla etkin aboneliklerin iptalini hızlandırın. Abonelikleri ve Azure aboneliklerini iptal Office 365 hakkında daha fazla bilgi edinin. Bir kiracıyla ilişkilendirme veya var olan aboneliği ekleme hakkında yol gösterici bilgiler için bkz. Azure AD kiracınıza [Bir Azure aboneliğini ilişkilendirme veya ekleme](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Etkin lisans yok. Lisansları kaldırmak için bkz. [Lisansı Kaldırmak için Aboneliği Kaldırma](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Azure AD'ye silme girişiminde bulunurken Dizinde Genel Yönetici olarak kendiniz dışında başka etkin kullanıcı yok. Diğer tüm etkin kullanıcıları kaldırabilirsiniz ve kiracıda özel etki alanı adına bağımlılıkların (örneğin, etki alanıyla oluşturulan kullanıcılar) admin@contoso.com.

Şu adımların nasıl ayrıntılı olarak anlatılması gerekir:
- "Abonelik Azure Active Directory" veya "abonelik" ifadesini silme için bkz. [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)
- Dizinde uygulamaları kaldırma, bkz. [Uygulamaları Kaldırma](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
