---
title: iOS aygıtlarını Microsoft Intune'a kaydetme yle ilgili sorun giderme sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736178"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>iOS aygıtlarını Microsoft Intune'a kaydetme yle ilgili sorun giderme sorunları

Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirin. 
  
Bazı yaygın hata iletileri ve çözüm adımları:
  
- **Cihaz Kapağına Ulaşıldı** Kullanıcı, aygıt sınırından daha fazla aygıt alabilenir. [Aygıtı kaldırmak](https://docs.microsoft.com/intune/devices-wipe) veya aygıt [sınırını değiştirmek](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)için bu belgeleri gözden geçirin.
    
- **Bu Hizmet desteklenmez. Kayıt Politikası Yok:** Apple Push Bildirim Hizmeti'nin (APNS) yapılandırılması veya yenilenmesi gerekir. Bunun nasıl yapılacağını anlatan talimatlar için [bu belgeyi](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) gözden geçirin. 
    
- **Kullanıcı Lisans Türü Geçersiz veya Kullanıcı Adı Tanınmadı:** Kullanıcıya bir Intune veya EMS lisansı atanması gerekir. Lisans atamak için bu belgeleri gözden [geçirin: Office Yönetici Merkezi](https://docs.microsoft.com/intune/licenses-assign) veya [Azure portalı.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Sorununuzu çözmeye yardımcı olacak ek kaynaklar:
  
1. Sık karşılaşılan kayıt hatalarını tanılamak ve gidermek için [Intune Sorun Giderme Portalı'nı](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) kullanın. Daha fazla ayrıntı için [bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) gözden geçirin. 
    
2. Bu belgeleri, her birine kaydolmasını ve çözümlerini engelleyen yaygın hataların bir listesi için gözden geçirin: [Sorun Giderme kılavuzu](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ve [Sorun Giderme dokümanı.](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)
    
3. [iOS aygıtlarını Microsoft Intune'a nasıl kaydedebilirsiniz öğrenin.](https://docs.microsoft.com/intune/ios-enroll)
    

