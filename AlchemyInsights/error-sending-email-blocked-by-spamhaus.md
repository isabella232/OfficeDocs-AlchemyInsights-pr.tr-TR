---
title: SpamHaus tarafından engellenen bir e-posta gönderilirken hata oluştu
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783823"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>E-posta gönderilirken hata oluştu: Istemci ana bilgisayarı Spamhaus kullanılarak engellendi

İletiyi gönderen IP adresi, [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)'in sahip olduğu bir engelleme listesinde yer alıyor. Spamhaus tarafından engellenmesi nedenleri, genel bir IP adresi ve Internet servis sağlayıcısı (ISS) ilkelerini paylaşan güvenliği aşılan hesaplar, güvenliği aşılan makineler içeriyor. Olası düzeltmeler:
  
- Kaynak e-posta sunucusunu kontrol ettiğiniz engellenen gelen iletilerde, nedeni belirlemeniz ve bloğu Spamhaus Web sitesinden kaldırmanız gerekir.

- Kaynak IP adresinin başka birine ait olduğu engellenen gelen iletiler için, adresin sahibinin, Spamhaus Web sitesinden engellemeyi kaldırması gerekmektedir. IP adresi Ilke engelleme listesinde (PBL) yer alıyorsa, sahibi farklı bir statik IP adresi atayabilir veya bu adresi PBL 'den kaldırabilir.

- Microsoft 'a bağlı etki alanınızda engellenmiş giden iletiler için, iletiler üçüncü taraf bir hizmet üzerinden yönlendirildiyse bu hatayı alabilirsiniz. Engellenen IP adresi sahibini bulmak için bir WHOIS arama aracı kullanabilirsiniz.
