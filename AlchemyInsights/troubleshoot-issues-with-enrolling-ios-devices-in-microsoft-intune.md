---
title: Microsoft Intune 'da iOS cihazlarını kaydetme sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669268"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Microsoft Intune 'da iOS cihazlarını kaydetme sorunlarını giderme

Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirin. 
  
Bazı yaygın hata iletileri ve çözüm adımları:
  
- **Cihaz Cap 'e ulaşıldı** Kullanıcının cihaz sınırından daha fazla kayıtlı cihazı var. [Cihazı kaldırmak](https://docs.microsoft.com/intune/devices-wipe) veya [cihaz sınırını değiştirmek](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)için bu belgeleri gözden geçirin.
    
- **Bu hizmet desteklenmiyor. Kayıt Ilkesi yok:** Apple anında bildirim hizmeti (APNs) yapılandırılmalı veya yenilenmelidir. Bunun nasıl yapıldığını açıklayan yönergeler için [Bu belgeyi](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) inceleyin. 
    
- **Kullanıcı Lisans türü geçersiz veya Kullanıcı adı tanınmadı:** Kullanıcıya bir Intune veya EMS lisansı atanmalıdır. [Office Yönetim Merkezi](https://docs.microsoft.com/intune/licenses-assign) veya [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups)aracılığıyla lisans atamak için bu belgeleri gözden geçirin.
    
Sorununuzu çözmek için ek kaynaklar:
  
1. Yaygın kayıt hatalarını tanılamak ve çözmek için [Intune sorun giderme portalı](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 'nı kullanın. Daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) inceleyin. 
    
2. Her biri için kayıt ve çözünürlüğe engel olan yaygın hataların listesi için bu belgeleri gözden geçirin: [sorun giderme kılavuzu](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ve [belge sorunlarını giderme](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)
    
3. [Microsoft Intune 'Da iOS cihazlarını kaydettirme hakkında bilgi edinin](https://docs.microsoft.com/intune/ios-enroll).
    

