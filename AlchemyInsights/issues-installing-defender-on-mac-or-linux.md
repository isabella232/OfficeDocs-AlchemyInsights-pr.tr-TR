---
title: Mac veya Linux'ta Microsoft Defender'ı yükleme sorunları
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
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "50714319"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Mac veya Linux'ta Microsoft Defender'ı yükleme sorunları

**Mac**

- Mac için Microsoft Defender ATP'yi yüklemeden önce sistem gereksinimlerini karşılayanın. Daha fazla bilgi için [Bkz. Mac için Microsoft Defender ATP'yi yükleme.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Dosyada şu bilgileri gözden geçirebilirsiniz: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Linux için Microsoft Defender ATP'yi yüklemeden önce sistem gereksinimlerini karşılayanın. Daha fazla bilgi için [Linux için Microsoft Defender ATP'yi yükleme hakkında bilgi için bkz.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- MDATP hizmetinin çalıştığını doğrulamak için, yüklemenin başarısız [olduğunu doğrulayın.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Hizmet çalışmıyorsa sorunları gidermek ve gidermek için, [mdatp hizmeti çalışmıyorsa](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)sorun giderme adımlarına bakın.
- Ürünün durumunu doğrular ve EICAR metin dosyasında bir algılama testi çalıştırmak için istemci yapılandırmasını denetleme adımları için, İstemci [yapılandırmasına bakın.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)  

    **Not** Erişime açık etkinlikler için desteklenen dosya sistemlerinin listesi için Linux için [Microsoft Defender ATP'ye bakın.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)