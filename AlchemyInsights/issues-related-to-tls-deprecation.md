---
title: TLS 1.0 ve TLS 1.1 devre dışı bırakıı nedeniyle Office 365/e-posta gönderemiyor/e-posta alamıyor
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
- "9005383"
- "9275"
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054926"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>TLS 1.0 ve TLS 1.1 devre dışı bırakıı nedeniyle Office 365/e-posta gönderemiyor/e-posta alamıyor

MC229914, TLS 1.0 ve TLS 1.1 kullanımdanlanma sonrası ileti merkezi tarafından onaylandı ve Exchange Online uç noktaları için zorlama başlatıldı. Yakında Office 365 artık dış kaynaklardan gelen TLS 1.0 ve TLS 1.1 e-posta bağlantılarını kabulmayacak. Ayrıca, Exchange Online e-posta göndermek için hiçbir zaman TLS 1.0 veya 1.1 kullanmaz. TLS 1.0 veya 1.1 devre dışı bırakılıyorsa, aşağıdaki hatalardan birini kullanabilirsiniz:

- Gönderen NDR geri dönüyor - '421 4.4.2 Yuva Hata nedeniyle bağlantı bırakıldı'
- Officer 365- '421 4.4.2 SocketError nedeniyle bağlantı atıldı' e-postası gönderen Şirket İçi Sunucunun Kuyruk Görüntüleyicisi'nde hata
- Office 365- TLS görüşmesinde e-posta gönderen sunucuda Bağlayıcı Protokolü gönderme günlüğü hata YuvaError ile başarısız oldu [](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging)
- Bağlayıcı protokol günlüğü gönderme veya alma hatası - '451 5.7.3 Öncelikle STARTTLS komutu ve olmalı'

Yukarıdaki hatalardan herhangi birini görüyorsanız, lütfen e-posta gönderen veya alan sunucunun TLS 1.2'yi etkinleştirildiğinden emin olun.

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\İstemci] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Yukarıdaki kayıt defteri anahtarlarında TLS 1.2'yi etkinleştirmek için herhangi bir değişiklik yaptısanız değişikliklerin etkin olması için sunucuyu yeniden başlatın. Ayrıca, en son güncelleştirmelerin ve en Windows Exchange da yüklü olduğundan emin olun.

Daha fazla bilgi için bkz.:

- [Exchange Server TLS kılavuzu, bölüm 1: TLS 1.2 için Hazırlanıyor - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS kılavuzu Bölüm 2: TLS 1.2'yi Etkinleştirme ve Kullanmayan İstemcileri Belirleme - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [TLS sürümlerinin herhangi bir sürümle kabulı alınamazsa e-posta Exchange Online anlama - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
