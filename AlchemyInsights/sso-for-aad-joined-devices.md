---
title: Single-Sign Active Directory'ye katılmış cihazlar için daha fazla bilgi edinin
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405664"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Azure Active Directory'ye Katılan Cihazlar için çoklu oturum açma

Şirket içi Active Directory (AD) ortamınız varsa ve AD etki alanına katılmış bilgisayarlarınızı Azure AD'ye katılmak istiyorsanız, karma Azure AD birleştirmeyi yaparak bunu gerçekleştirebilirsiniz. [Nasıl Kullanılır: Karma Azure Active Directory birleştirme](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) uygulamanızı planlamak, ortamınıza karma bir Azure AD birleştirmesi uygulamayla ilgili adımlar sağlar.

[İş için Windows Hello kullanarak Şirket İçi Single-Sign Için Azure AD'ye katılmış cihazları yapılandırma](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Birincil Yenileme Belirteci (PRT) sorunları** Birincil Yenileme Belirteci (PRT), Windows 10, Windows Server 2016 ve sonraki sürümler, iOS ve Android cihazlarında Azure AD kimlik doğrulamasının önemli bir yapıdır. Bu, bu cihazlarda kullanılan uygulamalarda çoklu oturum açmayı (SSO) etkinleştirmek için Microsoft birinci taraf belirteç aracıları için özel olarak verilen bir JSON Web Belirtecidir (JWT). [Birincil Yenileme Belirteci nedir?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)Windows 10 cihazlarında BIR PRT'nin nasıl çıkar, kullanılır ve korunarak nasıl korunduğla ilgili ayrıntılar sağlarız.

**WamDefaultSet: YES ve AzureADPrt: YES** Bu alanlar, kullanıcının cihazda oturum a açması için Azure AD'de başarılı bir şekilde kimlik doğrulaması olup olmadığını gösterir. Değerler NO **ise,** son tarihi şu olabilir:

- Kayıt sırasında cihazla ilişkilendirilmiş OLAN TPM'de hatalı depolama anahtarı (yükseltilmiş çalışırken KeySignTest'i kontrol edin).
- Alternatif Oturum Açma Kimliği
- HTTP Proxy bulunamadı

dsregcmd komutunu kullanarak cihaz sorunlarını giderme - [SSO durumu](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
