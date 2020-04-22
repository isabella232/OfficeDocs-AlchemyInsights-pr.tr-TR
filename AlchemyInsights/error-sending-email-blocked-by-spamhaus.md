---
title: SpamHaus tarafından engellenen e-posta gönderme hatası
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714278"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>E-posta gönderme hatası: İstemci ana bilgisayar Spamhaus kullanılarak engellendi

İletiyi gönderen IP adresi [Spamhaus'a](https://go.microsoft.com/fwlink/p/?linkid=123245)ait bir blok listesindedir. Spamhaus tarafından engellenmesinin nedenleri arasında, gizliliği ihlal edilen hesaplar, genel BIR IP adresini paylaşan tehlikeye atılmış makineler ve Internet Servis Sağlayıcısı (ISS) ilkeleri yer almaktadır. Olası düzeltmeler şunlardır:
  
- Kaynak e-posta sunucusunu kontrol ettiğiniz engellenen gelen iletiler için nedenini belirlemeniz ve engellemeyi Spamhaus web sitesinden kaldırmanız gerekir.

- Kaynak IP adresinin başka birine ait olduğu engellenen gelen iletiler için adres sahibinin engellemeyi Spamhaus web sitesinden kaldırması gerekir. IP adresi İlke Blok Listesi'nde (PBL) yer alıyorsa, sahibi farklı bir statik IP adresi atayabilir veya adresi PBL'den kaldırabilir.

- Microsoft'a bağlı etki alanınızdan engellenen giden iletiler için, iletiler üçüncü taraf hizmeti aracılığıyla yönlendirilirse bu hatayı alabilirsiniz. Engellenen IP adresi sahibini bulmak için bir WHOIS arama aracı kullanabilirsiniz.
