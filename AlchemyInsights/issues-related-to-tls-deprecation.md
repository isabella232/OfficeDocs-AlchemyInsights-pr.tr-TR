---
title: TLS 1.0 ve TLS 1.1 devre dışı bırakılama nedeniyle Office 365'e e-posta gönderemiyor/alınamıyor
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
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747113"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>TLS 1.0 ve TLS 1.1 devre dışı bırakılama nedeniyle Office 365'e e-posta gönderemiyor/alınamıyor

MC229914 sonrası ileti merkezi tarafından onaylandırıldı ve TLS 1.0 ve TLS 1.1 kullanımdan çıktı. Yakında Office 365 dış kaynaklardan TLS 1.0 ve TLS 1.1 e-posta bağlantılarını kabul etmiyor. Ayrıca, Exchange Online giden e-posta göndermek için hiçbir zaman TLS 1.0 veya 1.1 kullanmaz. TLS 1.0 veya 1.1 devre dışı bırakıı nedeniyle sorunlar ile karşı karşıyaysanız, aşağıdaki hatalardan birini kullanabilirsiniz:

- Gönderen NDR geri geri dönüyor - '421 4.4.2 Yuva Hatana Bağlı Bağlantı bırakıldı'
- '421 4.4.2 SocketError' nedeniyle e-posta gönderen Şirket İçi Sunucusunun Sıra Görüntüleyicisi'nde hata oluştu
- Office 365'e e-posta gönderen sunucuda Bağlayıcı Protokolü Gönder günlüğünde hata oluştu- TLS görüşmeleri YuvaKor hatasıyla başarısız oldu [](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging)
- Bağlayıcı protokolü gönderme veya alma günlüğünde hata - '451 5.7.3 Önce STARTTLS komutu olmalı'

Yukarıdaki hatalardan herhangi birini görüyorsanız, lütfen e-posta gönderen veya alan sunucunun AŞAĞıDAKI kayıt defteri anahtarlarını kontrol ederek TLS 1.2'nin etkinleştirildiğinden emin olun:

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\İstemci] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Yukarıdaki kayıt defteri anahtarlarında TLS 1.2'yi etkinleştirmek için herhangi bir değişiklik yaptısanız, değişikliklerin etkin olması için sunucuyu yeniden başlatın. Ayrıca, en son Windows ve Exchange güncelleştirmelerinin yüklü olduğundan da emin olun.

Daha fazla bilgi için bkz.:

- [Exchange Server TLS kılavuzu, bölüm 1: TLS 1.2 için Hazırlanıyor - Microsoft Tech Topluluğu](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS kılavuzu Bölüm 2: TLS 1.2'yi etkinleştirme ve Kullan kullanmayan istemcileri tanımlama - Microsoft Tech Topluluğu](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [TLS sürümleri Exchange Online ile kabul edilemezse e-posta senaryolarını anlama - Microsoft Tech Topluluğu](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
