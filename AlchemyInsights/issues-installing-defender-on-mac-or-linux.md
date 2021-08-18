---
title: Mac veya Linux'a Microsoft Defender yükleme sorunları
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: defc11265caf371ce0a62a10a5de1d8ff88a8e11
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325269"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Mac veya Linux'a Microsoft Defender yükleme sorunları

**Mac**

- Mac için Microsoft Defender ATP'yi yüklemeden önce sistem gereksinimlerini karşılayanın. Daha fazla bilgi için [bkz. Mac için Microsoft Defender ATP'yi yükleme.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Dosyada bilgileri gözden geçirme: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Linux için Microsoft Defender ATP'yi yüklemeden önce sistem gereksinimlerini karşılayanın. Daha fazla bilgi için [bkz. Linux için MDATP yükleme.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- MDATP hizmetinin çalıştığını doğrulamak için bkz. [Yükleme başarısız.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Hizmet çalışmıyorsa sorunları gidermek ve gidermek için bkz. [Mdatp hizmeti](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)çalışmıyorsa giderme adımları .
- Ürünün durumunu doğrular ve EICAR metin dosyasında bir algılama testi çalıştırmak için istemci yapılandırmasını denetleme adımları için bkz. [İstemci yapılandırması](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Not** Erişime açık etkinlik için desteklenen dosya sistemlerinin listesi için bkz. Linux için [Microsoft Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).