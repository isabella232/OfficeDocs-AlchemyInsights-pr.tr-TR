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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483087"
---
# <a name="password-synchronization"></a>Parola eşitleme

**Parola Karma Eşitlemesi hiç çalışmıyor**

Parola Karması Eşitlemesi çalışmaması sırasında müşterilerin sık karşılaştığı bazı sorunlar:

- Şirket içi Active Directory ile iletişim kurmak için Azure AD Connect  tarafından kullanılan  Active Directory hesabına Dizin Değişikliklerini Çoğalt ve Dizin Değişikliklerini Çoğalt (parola eşitlemesi için gerekli olan tüm izinler) verilmmektedir. Bu izinleri Active Directory hesabına vererek bunu düzeltmeniz gerekir.
- Yönetici, Kullanıcı Sign-In yöntemini Parola Eşitlemesi'nden  Azure AD Connect sihirbazında **AD FS** ile Federasyon gibi başka bir seçenenle  değiştirdikten sonra parola karması eşitlemesi devre dışı bırakılır. Azure AD Connect sihirbazında parola karması eşitleme özelliğini yeniden etkinleştirerek bunu düzeltebilirsiniz.
- Şirket içi Active Directory ile bağlantı sorunu. Örneğin, bazı etki alanı denetleyicilerine Azure AD Connect [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) tarafından erişilemiyor veya gereken bağlantı noktaları Güvenlik Duvarı tarafından engellenmiş durumdadır. Azure AD Connect sunucusuyla şirket içi Active Directory arasındaki bağlantının doğru şekilde çalışmalarından emin olarak bu sorunu çözmeniz gerekir.
- Azure AD Connect sunucusu şu anda hazırlama modundadır ve bu da sunucunun parola karmalarını alamamasıdır - Sorunu gidermek için, Azure AD Connect eşitlemesi ile parola eşitlemesi sorunlarını giderme bölümünde açıklanan adımları izleyin - Hiçbir parola [eşitlenmez.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

**Parola Karma Eşitlemesi bazı kullanıcılarım için çalışmıyor**

1. Parola karması kullanıcı için eşitlenemezse, sorunu  araştırmak ve çözmek için Azure AD Connect'te sorun giderme görevini kullanın. Aşağıdaki görevleri gerçekleştirin:

    a. [Sihirbazda sorun giderme görevini çalıştırma](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Belirli bir kullanım için parola karması eşitleme sorunlarını araştırmak üzere sorun giderme cmdlet'ini kullanın](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Kullanıcı için şirket içi Active Directory Kullanıcı nesnesi etkinleştirildiğinde, **sonraki oturum açma seçeneğinde parolayı değiştirmesi** gerekir. Bu seçenek etkinleştirildiğinde, kullanıcıya geçici bir parola atanır ve bir sonraki oturum açma sırasında parolayı değiştirmesi istenir. Azure AD Connect, Geçici parolaları Azure AD'ye eşitlemez.

Yukarıdaki sorunu çözmek için, aşağıdaki görevlerden birini gerçekleştirin:

- Kullanıcıdan şirket içi uygulamada (örneğin, Windows Masaüstü) oturum açmasını ve parolayı değiştirmesini iste. Yeni parola Azure AD ile eşitlenir.
- Yöneticinin, Kullanıcı'nın bir sonraki oturum açma sırasında parolasını değiştirmesi ve yeni parolayı kullanıcıyla paylaşması seçeneğini etkinleştirmeden kullanıcının parolasını güncelleştirmesini sağlamak.

3. Şirket içi Active Directory Kullanıcı nesnesi nesne **eşitlemesi veya** parola eşitlemesi için doğru yapılandırılmamış. Bu sorunu gidermek için, Azure AD Connect eşitlemesi ile Parola karma eşitlemesi [sorunlarını giderme konusunda açıklanan adımları izleyin.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







