---
title: Microsoft Intune'da iOS cihazlarını kaydetmeyle ilgili sorunları giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823483"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Microsoft Intune'da iOS cihazlarını kaydetmeyle ilgili sorunları giderme

Sorununuzu çözmek için aşağıda listelenen kaynakları gözden geçirebilirsiniz. 
  
Sık karşılaşılan bazı hata iletileri ve çözüm adımları:
  
- **Cihaz Başlığına Ulaşıldı** Kullanıcının cihaz sınırının üzerinde kayıtlı cihazı var. Cihazı kaldırmak veya [cihaz sınırını değiştirmek için](https://docs.microsoft.com/intune/devices-wipe) bu belgeleri gözden [geçirebilirsiniz.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Bu Hizmet desteklenmiyor. Kayıt İlkesi Yok:** Apple Anında Bildirim Hizmeti (APNS) yapılandırıldığında veya yenilenmesi gerekir. Bunu [nasıl yapmaya](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) yönelik yönergeler için bu belgeyi gözden geçirebilirsiniz. 
    
- **Kullanıcı Lisans Türü Geçersiz veya Kullanıcı Adı Tanınmıyor:** Kullanıcıya Intune veya EMS lisansı atanıyor olması gerekir. Lisans atamak için şu belgeleri gözden geçirebilirsiniz: [Office Yönetim Merkezi](https://docs.microsoft.com/intune/licenses-assign) veya Azure [portalı.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Sorununuzu çözmenize yardımcı olacak ek kaynaklar:
  
1. Yaygın kayıt sorunlarını tanılamak ve gidermek için [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) Sorun Giderme Portalı'nın kullanın. Daha [fazla ayrıntı için](https://docs.microsoft.com/intune/help-desk-operators) bu belgeyi gözden geçirebilirsiniz. 
    
2. Kayıt ve çözümleri engelleyen yaygın hataların listesi için bu belgeleri gözden geçirebilirsiniz: Sorun giderme [kılavuzu](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ve [Sorun giderme belgesi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Microsoft Intune'da iOS cihazlarını kaydetmeyi öğrenin.](https://docs.microsoft.com/intune/ios-enroll)
    

