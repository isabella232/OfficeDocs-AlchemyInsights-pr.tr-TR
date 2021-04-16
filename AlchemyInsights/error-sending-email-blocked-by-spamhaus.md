---
title: SpamHaus tarafından engellenen e-posta gönderme hatası
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813744"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>E-posta gönderme hatası: İstemci ana bilgisayarı Spamhaus kullanılarak engellendi

İletiyi gönderen IP adresi Spamhaus'un engellenenler [listesinde yer alıyor.](https://go.microsoft.com/fwlink/p/?linkid=123245) Güvenliği tehlikeye atılmış hesaplar, ortak IP adresini paylaşarak güvenliği tehlikeye makineler ve İnternet Servis Sağlayıcısı (ISS) ilkeleri Spamhaus'un engelleme nedenlerinden bazılarıdır. Olası düzeltmeler:
  
- Kaynak e-posta sunucusunu kontrol etmek istediğiniz engellenen gelen iletiler için engelin nedenini belirlemeli ve engeli Spamhaus web sitesinden kaldırabilirsiniz.

- Kaynak IP adresinin başka birine ait olduğu engellenen gelen iletiler için adres sahibinin engeli Spamhaus web sitesinden kaldırması gerekir. IP adresi İlke Engelleme Listesi'de (PBL) yer alıyorsa, IP adresinin sahibi farklı bir statik IP adresi atayan veya adresi PBL'den kaldırabilir.

- İletiler bir üçüncü taraf hizmeti tarafından yönlendirildiyse, etki alanınıza bağlı olan engellenmiş giden iletiler için bu hatayı alabilirsiniz. Engellenmiş IP adresinin sahibini bulmak için WHOIS arama aracını kullanabilirsiniz.
