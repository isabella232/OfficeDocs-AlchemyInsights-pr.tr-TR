---
title: Parola eşitleme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960855"
---
# <a name="password-synchronization"></a>Parola eşitleme

**Parola Karma Eşitlemesi hiç çalışmıyor**

Parola Karma Eşitlemesi çalışmaması sırasında müşterilerin sık karşılaştığı bazı sorunlar:

- Azure AD Bağlan tarafından şirket içi Active Directory ile iletişim kurmak için kullanılan  Active Directory  hesabına Dizin Değişikliklerini Çoğalt ve Dizin Değişikliklerini Çoğalt Parola eşitlemesi için gerekli olan tüm izinler ; Active Directory hesabına bu izinleri vererek bunu çözmeniz gerekir.
- Yönetici Kullanıcı Sign-In yöntemini Parola Eşitlemesi'nden Azure  AD Bağlan sihirbazında **AD FS** ile Federasyon gibi başka bir seçense değiştirdikten sonra parola  karması eşitlemesi devre dışı bırakılır - Azure AD Bağlan sihirbazında parola karması eşitleme özelliğini yeniden etkinleştirerek bunu düzeltebilirsiniz.
- Şirket içi Active Directory ile ilgili bağlantı sorunu. Örneğin, bazı etki alanı denetleyicilerine Azure AD Bağlan tarafından [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) erişilemez veya gerekli bağlantı noktaları Güvenlik Duvarı tarafından engellenir - Azure AD Bağlan sunucusuyla şirket içi Active Directory arasındaki bağlantının doğru şekilde çalışır durumda olduğundan emin olarak bunu düzeltmeniz gerekir.
- Azure AD Bağlan sunucusu şu anda hazırlama modundadır ve bu da sunucunun parola karmaları arasında sorun gidermesine neden olur: Sorunu gidermek için [Azure AD Bağlan](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)eşitlemesi ile parola eşitlemesi sorunlarını giderme - Parola eşitlenmedi bölümünde açıklanan adımları izleyin.

**Parola Karma Eşitlemesi bazı kullanıcılarım için çalışmıyor**

1. Parola karmanın bir kullanıcı için eşitlene olmadığını  fark ettiyseniz, sorunu araştırmak ve çözmek için Azure AD Bağlan sorun giderme görevini kullanın. Aşağıdaki görevleri gerçekleştirin:

    a. [Sihirbazda sorun giderme görevini çalıştırma](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Belirli bir kullanım için parola karması eşitleme sorunlarını araştırmak üzere sorun giderme cmdlet'ini kullanın](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Kullanıcı için şirket içi Active Directory Kullanıcı nesnesi etkinleştirildiğinde, **bir sonraki oturum açma seçeneğinde parolayı değiştirmesi** gerekir. Bu seçenek etkinleştirildiğinde, kullanıcıya geçici bir parola atanır ve bir sonraki oturum açma sırasında kullanıcıdan parolayı değiştirmesi istenir. Azure AD Bağlan, geçici parolaları Azure AD'ye eşitlemez.

Yukarıdaki sorunu çözmek için, aşağıdaki görevlerden birini yapın:

- Kullanıcıdan şirket içi uygulamada oturum açmasını (örneğin, Masaüstü Windows) ve parolayı değiştirmesini iste. Yeni parola Azure AD'ye eşitlenir.
- Yöneticinin, Kullanıcı sonraki oturum açma sırasında parolayı değiştirmesi ve yeni parolayı kullanıcıyla paylaşması seçeneğini etkinleştirmeden kullanıcının parolasını güncelleştirmesini sağlar.

3. Şirket içi Active Directory Kullanıcı nesnesi, nesne **eşitlemesi veya parola eşitlemesi** için doğru yapılandırılmamış. Bu sorunu gidermek için, Azure AD ile parola karması eşitlemesi sorunlarını giderme [makalesinde açıklanan Bağlan izleyin.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







