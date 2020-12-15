---
title: Bekleme durumunda cihaz
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
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679995"
---
# <a name="device-in-pending-state"></a>Bekleme durumunda cihaz

**Koşullar**

1. Cihaz kayıtlarını ilk kez ayarlıyorsanız, Azure AD 'nın altındaki cihazları nasıl edindiğinize yol gösterecek olan [Azure Active Directory 'de (Azure AD) cihaz yönetimine giriş](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) konusunda gözden geçirdiğinizden emin olun.
2. Cihazları Azure AD 'ye doğrudan kaydedip Intune 'a kaydettirirken, [Intune 'u yapılandırdığınızdan](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ve öncelikle [Lisans](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) 'ı kullandığınızdan emin olmanız gerekir.
3. Azure AD ve şirket içi AD 'de işlemleri gerçekleştirme yetkiniz olduğundan emin olun. Yalnızca Azure AD 'deki genel yönetici, cihaz kayıtlarında ayarları yönetebilir. Ayrıca, şirket içi Active Directory 'nizde otomatik kayıtları ayarlıyorsanız, Active Directory ve AD FS yöneticisi olmanız gerekir (uygulanabiliyorsa).

Karma Azure AD katılma kayıt süreci, aygıtların şirket ağında olmasını gerektirir. Ayrıca VPN üzerinden de çalışır, ancak bazı uyarılar vardır. Uzaktan çalışma durumları altında karma Azure AD katılma kaydı işlemini sorun giderme konusunda yardım almak için müşteriler duyduk.

**Bulut kimlik doğrulama ortamı (Azure AD parola karma eşitleme veya geçiş kimlik doğrulaması kullanılarak)**

Bu kayıt akışı, "eşitleme katılma" olarak da bilinir.

Kayıt işlemi sırasında neler olduğunu aşağıda bulabilirsiniz:

1. Windows 10, Kullanıcı cihazda oturum açtığında hizmet bağlantı noktası (SCP) kaydını bulur.

    1. Cihaz öncelikle kayıt defterinde (HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD], istemci tarafı SCP 'den kiracı bilgilerini almaya çalışır. Daha fazla bilgi için bkz [.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    1. Başarısız olursa, cihaz SCP 'den kiracı bilgilerini almak için şirket içi Active Directory ile iletişim kurar. SCP 'yi doğrulamak için bu [belgeye](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)başvurun.

    > [!NOTE]
    > Active Directory 'de SCP 'YI etkinleştirmeyi ve yalnızca istemci tarafı SCP 'YI ilk doğrulama için kullanmayı öneririz.

2. Windows 10, sistem bağlamı altındaki Azure AD ile iletişim kurmaya çalışır.

    Cihazın sistem hesabı altındaki Microsoft kaynaklarına erişip erişebildiğini, [test cihazı kayıt bağlantı betiğini](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)kullanarak doğrulayabilirsiniz.

3. Windows 10 kendinden imzalanan sertifika oluşturur ve şirket içi Active Directory 'de bilgisayar nesnesinin altında depolar. Bu, etki alanı denetleyicisine görüntülenecek satır gerektirir.

4. Sertifikası olan cihaz nesnesi Azure AD Connect aracılığıyla Azure AD ile eşitlenir. Eşitleme döngüyü varsayılan olarak her 30 dakikada bir, ancak Azure AD Connect 'in yapılandırmasına bağlıdır. Daha fazla bilgi için bu [belgeye](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)bakın.

5. Bu aşamada, konu aygıtını Azure portalının cihaz Blade altında "**Beklemede**" durumunda görebilmelisiniz.

6. Windows 10 ' da sonraki kullanıcı oturumunda, kayıt tamamlanmış olacaktır.

    > [!NOTE]
    > VPN kullanıyorsanız ve oturum kapatma/oturum açma/oturum açma Bunu yapmak için:
    >
    > `dsregcmd /join`Yönetici isteminde ya da bilgisayarınıza PSExec aracılığıyla uzaktan sorun.
    >
    > Örneğin: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Azure Active Directory cihaz kaydıyla ilgili yaygın sorunlar için, [CIHAZLAR SSS](https://docs.microsoft.com/azure/active-directory/devices/faq)bölümüne bakın.
