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
# <a name="troubleshoot-user-consent"></a>Kullanıcı onayı sorunlarını giderme

1. Son kullanıcıların Azure portalı veya PowerShell aracılığıyla uygulamalara nasıl izin vermiş olduğunu yapılandırabilirsiniz. Daha fazla bilgi için [Kullanıcı onayı ayarlarına](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) bakın.
1. Yönetici, tek bir kullanıcı adına temsilci izinlerine izin vermek için [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) 'yi de kullanabilir. Daha fazla bilgi için, [Kullanıcı adına erişim alma](https://docs.microsoft.com/graph/auth-v2-user)bölümüne bakın.
1. [Kullanıcı onayı hataları](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): Bu makalede, bir uygulamaya uyum sürecinde oluşabilecek hatalar açıklanır. Herhangi bir hata iletisi içermeyen beklenmeyen onay istemleriyle ilgili sorun yaşıyorsanız, [Azure AD Için kimlik doğrulama senaryolarını](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)inceleyin.