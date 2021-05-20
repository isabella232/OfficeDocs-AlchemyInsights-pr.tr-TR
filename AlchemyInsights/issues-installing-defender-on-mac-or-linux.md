---
title: Mac veya Linux üzerine Microsoft Defender yükleme sorunları
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
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539700"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Mac veya Linux üzerine Microsoft Defender yükleme sorunları

**Mac**

- Mac için Office'i yüklemeden önce sistem Microsoft Defender ATP karşı olduğundan emin olun. Daha fazla bilgi için [bkz. Mac için Microsoft Defender ATP yükleme](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Dosyada bilgileri gözden geçirme: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Linux için Microsoft Defender ATP yüklemeden önce sistem Microsoft Defender ATP karşı olduğundan emin olun. Daha fazla bilgi için [bkz. Linux için MDATP yükleme.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- Hizmet hizmetinin MDATP doğrulamak için bkz. [Yükleme başarısız.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Hizmet çalışmıyorsa sorunları gidermek ve gidermek için bkz. [Mdatp hizmeti](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)çalışmıyorsa giderme adımları .
- Ürünün durumunu doğrular ve EICAR metin dosyasında bir algılama testi çalıştırmak için istemci yapılandırmasını denetleme adımları için bkz. [İstemci yapılandırması](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Not** Erişime açık etkinlikler için desteklenen dosya sistemlerinin listesi için Linux için [Microsoft Defender ATP'e bakın.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)