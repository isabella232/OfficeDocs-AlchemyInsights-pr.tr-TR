---
title: Cihaz beklemede durumda
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
- "9003244"
- "7319"
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330392"
---
# <a name="device-in-pending-state"></a>Cihaz beklemede durumda

**Önkoşullar:**

1. Cihaz kayıtlarını ilk kez ayarıyorsanız, cihazları Azure AD'nin denetimi altına nasıl alamazsanız size yol sağlayacak [olan Azure Active Directory'te (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) cihaz yönetimine giriş'i gözden geçirmeyi gözden geçirmeyi lütfen unutmayın.
2. Cihazları doğrudan Azure AD'ye kaydedecek ve bunları Intune'a kaydedeceksanız, [Intune'u](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) yapılandırmış ve lisansa ilk siz sahip olmak zorunda olursanız. [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)
3. Azure AD'de ve şirket içi AD'de işlem gerçekleştirme yetkiniz olduğundan emin olmak. Microsoft Azure AD’de yalnızca bir genel yönetici cihaz kayıtlarıyla ilgili ayarları yönetebilir. Ek olarak, şirket içi Active Directory’de otomatik kayıtlar ayarlıyorsanız, (mümkünse) Active Directory ve AD FS yöneticisi olmanız gerekir.

Karma Azure AD katılma kayıt işlemi, cihazların şirket ağına sahip olması gerekir. VPN üzerinden de çalışır, ancak bunun için bazı uyarılar vardır. Uzak çalışma durumlarına göre karma Azure AD birleştirme kayıt işlemiyle ilgili sorun giderme konusunda yardıma ihtiyaç duyan müşteriler olduğunu duyduk.

**Bulut kimlik doğrulama ortamı (Azure AD parola karma eşitlemesi veya geçişli kimlik doğrulaması kullanılarak)**

Bu kayıt akışı, "Katılma Eşitleme" olarak da bilinir.

Kayıt işlemi sırasında yapılan işlemlerin dökümü şöyledir:

1. Windows 10, kullanıcı cihazda oturum açtığında Hizmet Bağlantı Noktası (SCP) kaydını bular.

    1. Cihaz önce kayıt defterinde istemci tarafı SCP'den kiracı bilgilerini almaya çalışır [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Daha fazla bilgi için belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    1. Başarısız olursa, cihaz SCP'den kiracı bilgilerini almak için şirket içi Active Directory ile iletişim kurar. SCP'yi doğrulamak için bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    **Not:** Active Directory'de SCP'yi etkinleştirmenizi ve ilk doğrulama için yalnızca istemci tarafı SCP'yi etkinleştirmenizi öneririz.

2. Windows 10, kimlik doğrulaması için sistem bağlamı kapsamında Azure AD ile iletişim kurmaya çalışır.

    Cihazın sistem hesabı altındaki Microsoft kaynaklarına erişeni, Cihaz Kayıt Bağlantısını Test Edin [betiğiyle doğrulayasınız.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 otomatik olarak imzalanan sertifika oluşturur ve bunu şirket içi Active Directory'de bilgisayar nesnesi altında depolar. Bunun için Etki Alanı Denetleyicisi'nin görüş çizgisi gerekir.

4. Sertifikası olan cihaz nesnesi, Azure AD veya Azure AD aracılığıyla Azure AD ile Bağlan. Eşitleme döngüsü varsayılan olarak her 30 dakikada bir, ancak Azure AD etki alanı yapılandırma Bağlan. Daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Bu aşamada, Azure Portal'ın Cihaz blade'i altında konu cihazı **"** Beklemede " durumuna bakabilirsiniz.

6. Oturum açma işleminin bir Windows 10 sırasında kayıt tamamlanır.

    **Not:** VPN'niz varsa ve logoff/login etki alanı bağlantısını sonlandırılırsa, kaydı el ile tetikleyebilirsiniz. Bunu yapmak için:
    
    Yönetici `dsregcmd /join` istemine yerel olarak veya bilgisayarınıza PSExec aracılığıyla uzaktan bir sorun sorun.\
    Örneğin: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Cihaz kaydı sırasında karşılaşılan en Azure Active Directory için Cihazlar hakkında SSS [bölümüne bakın.](https://docs.microsoft.com/azure/active-directory/devices/faq)
