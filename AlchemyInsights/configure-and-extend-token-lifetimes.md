---
title: Belirteç ömürleri yapılandırma ve genişletme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917199"
---
# <a name="configure-and-extend-token-lifetimes"></a>Belirteç ömürleri yapılandırma ve genişletme

Microsoft Identity platform tarafından verilen bir Access, SAML veya KIMLIK belirtecinin ömrünü belirtebilirsiniz. Kuruluşunuzdaki tüm uygulamalar için, birden çok kiracı (çok kuruluş) uygulaması veya kuruluşunuzdaki belirli bir hizmet sorumlusu için belirteç ömürleri ayarlayabilirsiniz. Daha fazla bilgi için [yapılandırılabilir belirteç ömürleri](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)makalesini okuyun.

Örnekler için, [belirteç ömürleri yapılandırma ile ilgili örnekleri](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)okuyun.

Azure Active Directory B2C 'de bir simgenin kullanım ömrünü ve uyumluluğunu nasıl yapılandıracağınızı öğrenmek için, [Azure Active DIRECTORY B2C 'de belirteçleri yapılandırma](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)bölümüne bakın.

[Azure Active Directory 'de oturum davranışını yapılandırma](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) : Azure AD B2C 'de kullanılan çoklu oturum açma (SSO) yöntemlerini açıklar ve ilkenizi yapılandırırken en uygun SSO yöntemini seçmenize yardımcı olur.

**Ne kadar çok simge kullanıyorsunuz? Ne kadar sürer?**

Belirteç ömürleri 1 saat ve oturum yaşam süresi 24 saattir. Bu, 24 saat içinde hiçbir istekte bulunulmadığı durumlarda, yeni bir belirteç istemeden önce yeniden oturum açmanız gerekir.

> [!NOTE]
> 30 Mayıs 2020 ' den sonra, oturum ve yenileme belirteçlerini yapılandırma Kullanımdan kalkma, var olan oturum ve yenileme belirteçleri ilkeleriyle bu kadar çok ay içinde gerçekleşecektir. Yine de erişim belirteci ömürleri 'ni kullanımdan kaldırma.






