---
title: Microsoft Intune IOS aygıtları kaydolma sorunları giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507023"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Microsoft Intune IOS aygıtları kaydolma sorunları giderme

Şimdi, sorunu gidermek için aşağıda listelenen kaynakları inceleyin. 
  
Bazı yaygın hata iletileri ve çözümleme adımları:
  
- **Aygıt Cap ulaştı** Daha fazla aygıtlar Aygıt üst sınırından kayıtlı kullanıcı vardır. [Bir aygıtı kaldırmak](https://docs.microsoft.com/intune/devices-wipe) veya [aygıt bu sınırı değiştirmek](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)için bu belgeleri gözden geçirin.
    
- **Bu hizmeti desteklenmiyor. Hiçbir kayıt ilkesi:** yapılandırılmış veya yenilenmiş elma itme bildirim hizmeti (APNS) gerekir. Bunu yapmak yönergeler için [Bu belgeyi](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) gözden geçirin. 
    
- **Kullanıcı lisans türü geçersiz veya tanınmayan kullanıcı adı:** Kullanıcı bir Intune veya EMS lisans atanması gerekir. Bir lisans aracılığıyla atamak için bu belgeleri gözden geçirin: [Office Yönetim Merkezi](https://docs.microsoft.com/intune/licenses-assign) veya [Azure portalı](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Sorununuzu gidermeye yardımcı olmak için ek kaynaklar:
  
1. [Intune sorun giderme Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) tanılamak ve ortak kayıt hatalarını gidermek için kullanın. Daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) gözden geçirin. 
    
2. Bu belgeler için kayıt ve çözümler için her önlemek sık karşılaşılan hataların listesini gözden geçirin: [sorun giderme kılavuzu](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ve [sorun giderme doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Microsoft Intune IOS aygıtları kaydetmek öğrenin](https://docs.microsoft.com/intune/ios-enroll).
    

