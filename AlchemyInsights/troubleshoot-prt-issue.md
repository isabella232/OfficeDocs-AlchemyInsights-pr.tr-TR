---
title: PRT sorunu giderme
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
ms.openlocfilehash: a005c4a6848bbf0725560375df1220ce906cbb5f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330979"
---
# <a name="troubleshoot-prt-issue"></a>PRT sorunu giderme

Herhangi bir cihazın kimlik doğrulama işlemini tamamlaması için cihazın tümüyle kaydedilmiş ve iyi durumda olması ve Birincil Yenileme Belirteci'nin (PRT) edinilmiş olması gerekir.

Karma Azure AD katılma kayıt işlemi, cihazların şirket ağına katılmasını gerektirir. VPN üzerinden de çalışır, ancak bunun için bazı uyarılar vardır. Uzak çalışmalı koşullarda karma Azure AD birleştirme kayıt işlemiyle ilgili sorun giderme konusunda yardıma ihtiyaç duyan müşteriler olduğunu duyduk. Kayıt işlemi sırasında 'daha altta' olan işlemlerin dökümünü burada açıklarız.

**Bulut kimlik doğrulama ortamı (Azure AD parola karma eşitlemesi veya geçişli kimlik doğrulaması kullanılarak)**

Bu kayıt akışı, "Katılma Eşitleme" olarak da bilinir.

1. Windows 10 kullanıcının cihazda oturum açması üzerine bir SCP kaydı keşfeder.
    1. Cihaz önce kayıt defterinde istemci tarafı SCP'den kiracı bilgilerini almaya çalışır [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    2. Başarısız olursa, cihaz Hizmet Bağlantı Noktası'dan (SCP) kiracı bilgilerini almak için şirket içi Active Directory (AD) ile iletişim kurar. SCP'yi doğrulamak için lütfen bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

**Not:** AD'de SCP'yi etkinleştirmenizi ve ilk doğrulama için yalnızca istemci tarafı SCP'yi etkinleştirmenizi öneririz.

2. Windows 10, kimlik doğrulaması için sistem bağlamı kapsamında Azure AD ile iletişim kurmaya çalışır. Cihazın sistem hesabı altındaki Microsoft kaynaklarına erişeni, Cihaz Kayıt Bağlantısını Test Edin betiğiyle doğru edebilirsiniz.

3. Windows 10 otomatik olarak imzalanan bir sertifika oluşturur ve bunu şirket içi AD'de bilgisayar nesnesi altında depolar. Bunun için Etki Alanı Denetleyicisi'nin görüş çizgisi gerekir.

4. Sertifikası olan bir cihaz nesnesi, Azure AD veya Azure AD tarafından Azure AD ile Bağlan. Eşitleme döngüsü varsayılan olarak her 30 dakikada bir ancak Azure AD'nin yapılandırmasına Bağlan. Daha fazla bilgi için lütfen bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Bu aşamada, Azure Portal'ın Cihaz blade'i altında konu cihazı "Beklemede" durumda görüyor olun.

6. Oturum açma işleminin bir Windows 10 sırasında kayıt tamamlanır. 

**Not:** VPN'niz varsa ve logolu oturum açma işlemi etki alanı bağlantısını sonlandırılırsa, kaydı el ile tetikleyebilirsiniz:
 1. Yönetici isteminde yerel olarak veya PC'nize PSExec aracılığıyla uzaktan bir dsregcmd /join sorun. Örneğin, PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Karma Katılma sorunları hakkında daha fazla ayrıntı için bkz. [Cihaz sorunlarını giderme.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
