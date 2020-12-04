---
title: Stok sorununu giderme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573904"
---
# <a name="troubleshoot-prt-issue"></a>Stok sorununu giderme

Herhangi bir cihazın kimliği doğrulanmış almayı tamamlamak için, tam olarak kaydedilmelidir ve iyi bir durumda ve birincil yenileme belirteci (PRT) edinebilmek gerekir.

Karma Azure AD katılma kayıt süreci, aygıtların şirket ağında olmasını gerektirir. Ayrıca VPN üzerinden de çalışır, ancak bazı uyarılar vardır. Uzaktan çalışma durumları altında karma Azure AD katılma kaydını sorun giderme konusunda yardım almak için müşteriler olduğunu duyduk. İşte, kayıt işlemi sırasında "çok yer

**Bulut kimlik doğrulama ortamı (Azure AD parola karma eşitleme veya geçiş kimlik doğrulaması kullanılarak)**

Bu kayıt akışı, "eşitleme katılma" olarak da bilinir.

1. Windows 10, kullanıcının cihazda oturum açarken bir SCP kaydını bulur.
    1. Cihaz öncelikle kayıt defterinde (HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD], istemci tarafı SCP 'den kiracı bilgilerini almaya çalışır. Daha fazla bilgi için bu [belgeye](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)bakın.
    2. Başarısız olursa, cihaz hizmet bağlantı noktasından (SCP) kiracı bilgilerini almak için şirket içi Active Directory (AD) ile iletişim kurar. SCP 'yi doğrulamak için lütfen bu [belgeye](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)başvurun. 

> [!NOTE]
> İlk doğrulama için AD içinde SCP 'YI etkinleştirip yalnızca istemci tarafı SCP 'YI kullanmayı öneririz.

2. Windows 10, sistem bağlamı altındaki Azure AD ile iletişim kurmaya çalışır. Cihazın sistem hesabı altındaki Microsoft kaynaklarına erişip erişebildiğini, test cihazı kayıt bağlantı betiğini kullanarak doğrulayabilirsiniz.

3. Windows 10 kendinden imzalanan bir sertifika oluşturur ve şirket içi AD 'de bilgisayar nesnesinin altında depolar. Bu, etki alanı denetleyicisine görüntülenecek satır gerektirir.

4. Azure AD Connect aracılığıyla, sertifikaya sahip bir cihaz nesnesi Azure AD ile eşitlenmiş. Eşitleme döngüyü varsayılan olarak her 30 dakikada bir, ancak Azure AD Connect 'in yapılandırmasına bağlıdır. Daha fazla bilgi için lütfen bu [belgeye](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)bakın.

5. Bu aşamada, konu aygıtını Azure portalının cihaz Blade altında "beklemede" durumunda görebilmelisiniz.

6. Windows 10 ' da sonraki kullanıcı oturumunda, kayıt tamamlanmış olacaktır. 

> [!NOTE]
> VPN kullanıyorsanız ve oturum kapatma işlemini etki alanı bağlantısını sona erdirirse, kaydı el ile tetikleyebilirsiniz:
 1. Bir dsregcmd/Join 'i yerel olarak yönetici isteminde veya PSExec aracılığıyla PC 'nize uzaktan yapın. Örneğin, PsExec-s \\ win10client01 cmd, dsregcmd/Join

 2. Karma birleşim [sorunlarıyla ilgili daha](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)fazla bilgi için bkz.
