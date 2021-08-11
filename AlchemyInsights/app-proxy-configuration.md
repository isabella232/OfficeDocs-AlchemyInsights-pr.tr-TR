---
title: Uygulama Ara Sunucusu Yapılandırması
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951585"
---
# <a name="app-proxy-configuration"></a>Uygulama Ara Sunucusu Yapılandırması

1. Uygulama Ara Sunucusu uygulamasını Azure AD'de şirket içi uygulamalarınızı buluta açık olacak şekilde yapılandırmayı anlamak için [bkz. Uygulama](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)Ara Sunucusu uygulamasını yapılandırma.
2. Çoklu oturum açma (SSO), kullanıcılarının bir uygulamaya birden çok kez kimlik doğrulama yapmadan erişmelerine olanak sağlar. Bu özellik, tek kimlik doğrulamasının bulutta Azure Active Directory izin verir ve hizmet veya Bağlayıcı'nın, uygulamanın ek kimlik doğrulama zorluklarını tamamlaması için kullanıcının kimliğine bürünmelerine olanak sağlar. Daha fazla bilgi edinmek için bkz. Uygulama Ara Sunucusu [uygulamasında çoklu oturum açma nasıl yapılandırılır.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)
3. Yeni [bir uygulama ara](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) sunucusu uygulaması oluştururken karşılaşılan yaygın sorunları gidermek için bu makaleyi kullanın.
4. Uygulamanıza arka uç kimlik doğrulamasını ayarlarken sorun ediyorsanız, sorununuzu çözmek için Uygulama Ara Sunucusu için [Kerberos'un](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) kısıtlanmış temsilci yapılandırmalarını gidermeniz veya [PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) ile uygulama yapılandırma yönergelerini izlemeniz gerekir.
