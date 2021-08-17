---
title: Single-Sign katıldığınız Azure Active Directory için daha fazla bağlantı
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
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050030"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Katıldığınız Cihazlar için Azure Active Directory oturum açma

Şirket içi Active Directory (AD) ortamınız varsa ve AD etki alanına katılmış bilgisayarlarınızı Azure AD'ye katılmak için, karma Azure AD birleştirmeyi yaparak bunu gerçekleştirebilirsiniz. [Nasıl İlgili: Karma Azure Ad Azure Active Directory planlama,](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) ortamınıza karma bir Azure AD birleştirmesi uygulamak için ilgili adımları sağlar.

[Windows Hello For Business kullanarak Şirket içi cihazlar için Azure AD'ye Single-Sign cihazları yapılandırma](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Birincil Yenileme Belirteci (PRT) sorunları** Birincil Yenileme Belirteci (PRT), Windows 10, Windows Server 2016, iOS ve Android cihazlarında Azure AD kimlik doğrulamasının önemli bir yapıdır. Bu, bu cihazlarda kullanılan uygulamalarda çoklu oturum açma (SSO) özelliği sağlamak için microsoft birinci taraf belirteç aracıları için özel olarak bir JSON Web Belirteci (JWT) verir. [Birincil Yenileme Belirteci nedir?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)altında, farklı cihazlarda PRT'nin nasıl konuldu, kullanıldı ve Windows 10 sağlarız.

**WamDefaultSet: YES ve AzureADPrt: YES** Bu alanlar, cihazda oturum a açmada kullanıcının Azure AD'ye başarıyla kimlik doğrulaması edip olmadığını gösterir. Değerler NO **ise,** bunun nedeni şu olabilir:

- Kayıt sırasında cihazla ilişkilendirilmiş TPM'de kötü depolama anahtarı (yükseltilmiş çalışırken KeySignTest'i kontrol edin).
- Alternatif Oturum Açma Kimliği
- HTTP Proxy bulunamadı

dsregcmd komutunu - [SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state) durumunu kullanarak cihaz sorunlarını giderme
