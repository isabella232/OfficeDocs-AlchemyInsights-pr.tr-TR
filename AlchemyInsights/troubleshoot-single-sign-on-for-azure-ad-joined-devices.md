---
title: Azure AD'ye Katılan Cihazlar için Çoklu oturum açma sorunlarını giderme
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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037336"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Azure AD'ye Katılan Cihazlar için Çoklu oturum açma sorunlarını giderme

Şirket içi Active Directory (AD) ortamınız varsa ve AD etki alanına katılmış bilgisayarlarınızı Azure AD'ye katılmak istiyorsanız, karma Azure AD birleştirmeyi yaparak bunu gerçekleştirebilirsiniz. [Nasıl Kullanılır: Karma Azure Active Directory birleştirme](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) uygulamanızı planlamak, ortamınıza karma bir Azure AD birleştirmesi uygulamayla ilgili adımlar sağlar.

Daha fazla bilgi için bkz. Şirket içi Single-Sign İş için Windows Hello kullanırken [Azure AD'ye katılmış cihazları yapılandırma.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Birincil Yenileme Belirteci (PRT) sorunları**

Birincil Yenileme Belirteci (PRT), Windows 10, Windows Server 2016 ve sonraki sürümler, iOS ve Android cihazlarında Azure AD kimlik doğrulamasının önemli bir yapıdır. Bu, bu cihazlarda kullanılan uygulamalarda çoklu oturum açmayı (SSO) etkinleştirmek için Microsoft birinci taraf belirteç aracıları için özel olarak verilen bir JSON Web Belirtecidir (JWT). Windows 10 cihazlarında BIR PRT'nin nasıl çıkarı, kullanılır ve korunarak nasıl korunmaktadır hakkında ayrıntılı bilgi için bkz. Birincil Yenileme [Belirteci nedir?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

**WamDefaultSet: YES ve AzureADPrt: YES**

Bu alanlar, kullanıcının cihazda oturum a açması için Azure AD'de başarılı bir şekilde kimlik doğrulaması olup olmadığını gösterir. Değerler NO **ise,** bunun nedeni şu olabilir:

- Kayıt sırasında cihazla ilişkilendirilmiş OLAN TPM'de hatalı depolama anahtarı (yükseltilmiş çalışırken KeySignTest'i kontrol edin)
- Alternatif Oturum Açma Kimliği
- HTTP Proxy bulunamadı

dsregcmd komutunu kullanarak cihaz sorunlarını gidermek için [SSO durumuna bakın.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
