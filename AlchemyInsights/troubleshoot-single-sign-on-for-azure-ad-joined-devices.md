---
title: Azure AD'ye Katılmış Cihazlar için Çoklu oturum açma sorunlarını giderme
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
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039266"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Azure AD'ye Katılmış Cihazlar için Çoklu oturum açma sorunlarını giderme

Şirket içi Active Directory (AD) ortamınız varsa ve AD etki alanına katılmış bilgisayarlarınızı Azure AD'ye katılmak için, karma Azure AD birleştirmeyi yaparak bunu gerçekleştirebilirsiniz. [Nasıl İlgili: Karma Azure Ad Azure Active Directory planlama,](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) ortamınıza karma bir Azure AD birleştirmesi uygulamak için ilgili adımları sağlar.

Daha fazla bilgi için bkz. Azure AD'ye katılmış cihazları Şirket içi cihazlar [için yapılandırma Single-Sign Windows Hello Kullanarak.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Birincil Yenileme Belirteci (PRT) sorunları**

Birincil Yenileme Belirteci (PRT), Windows 10, Windows Server 2016, iOS ve Android cihazlarında Azure AD kimlik doğrulamasının önemli bir yapıdır. Bu, bu cihazlarda kullanılan uygulamalarda çoklu oturum açma (SSO) özelliği sağlamak için microsoft birinci taraf belirteç aracıları için özel olarak bir JSON Web Belirteci (JWT) verir. Bir PRT'nin farklı cihazlarda nasıl çıkarlı olduğu, Windows 10 korunarak nasıl korunduğ hakkında ayrıntılı bilgi için bkz. Birincil Yenileme [Belirteci nedir?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES ve AzureADPrt: YES**

Bu alanlar, cihazda oturum a açmada kullanıcının Azure AD'ye başarıyla kimlik doğrulaması edip olmadığını gösterir. Değerler NO **ise,** bunun nedeni şu olabilir:

- Kayıt sırasında cihazla ilişkilendirilmiş TPM'de kötü depolama anahtarı (yükseltilmiş durumdayken KeySignTest'i kontrol edin)
- Alternatif Oturum Açma Kimliği
- HTTP Proxy bulunamadı

dsregcmd komutunu kullanarak cihazların sorunlarını gidermek için bkz. [SSO durumu.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
