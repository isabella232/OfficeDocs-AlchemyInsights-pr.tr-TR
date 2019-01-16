---
title: SpamHaus tarafından engellenen e-posta gönderme hatası
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28318185"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>E-posta gönderilirken hata: istemci ana bilgisayar Spamhaus kullanılarak engellendi

[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)tarafından sahip olunan bir engelleme listesindeki iletiyi gönderen IP adresi var. Spamhaus tarafından engellenmesini için nedenleri ele geçirilen hesapları, ortak bir IP adresi ve Internet servis sağlayıcısı (ISS) ilkelerini paylaşma makineleri tehlikeye. Olası düzeltmeler şunlardır:
  
- Office kaynak e-posta sunucusu kontrol burada 365 engellenen gelen iletiler için nedenini belirlemek ve blok Spamhaus Web sitesinden kaldırmak gerekir.
    
- Kaynak IP adresini başka bir kişiye ait olduğu Office 365 engellenen gelen iletiler için adres sahibi blok Spamhaus Web sitesinden kaldırmak gerekir. IP adresi İlkesi engelleme listesi (PBL) ise, sahibi PBL adresi kaldırın veya farklı bir statik IP adresi atayın.
    
- Office 365 etki alanınızdan engellenen giden iletiler için bu hata iletileri bir 3 parti hizmeti üzerinden yönlendirilir alabilir. Engellenen IP adresi sahibi bulmak için bir WHOIS arama aracını kullanabilirsiniz.
    

