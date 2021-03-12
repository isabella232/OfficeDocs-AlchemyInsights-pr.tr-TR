---
title: Microsoft Intune'da iOS cihazlarını kaydetmeyle ilgili sorunları giderme
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
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708982"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Microsoft Intune'da iOS cihazlarını kaydetmeyle ilgili sorunları giderme

Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirebilirsiniz. 
  
Sık karşılaşılan bazı hata iletileri ve çözüm adımları:
  
- **Cihaz Başlığına Ulaşıldı** Kullanıcının cihaz sınırının üzerinde kayıtlı cihazı var. Bir cihazı kaldırmak veya [cihaz sınırını değiştirmek](https://docs.microsoft.com/intune/devices-wipe) için bu belgeleri gözden [geçirebilirsiniz.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Bu Hizmet desteklenmiyor. Kayıt İlkesi Yok:** Apple Anında Bildirim Hizmeti'nin (APNS) yapılandırılması veya yenilenmesi gerekir. Bunu [nasıl yapacağıma](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) ilişkin yönergeler için bu belgeyi gözden geçirebilirsiniz. 
    
- **Kullanıcı Lisans Türü Geçersiz veya Kullanıcı Adı Tanınmıyor:** Kullanıcıya Intune veya EMS lisansı atanıyor olması gerekir. Şu belgeleri gözden geçirerek lisans atabilirsiniz: [Office Yönetim Merkezi veya](https://docs.microsoft.com/intune/licenses-assign) Azure [portalı.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Sorununuzu çözmenize yardımcı olacak ek kaynaklar:
  
1. Yaygın [kayıt hatalarını tanılamak ve](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) çözmek için Intune Sorun Giderme Portalı'nın kullanın. Daha [fazla ayrıntı için](https://docs.microsoft.com/intune/help-desk-operators) bu belgeyi gözden geçirebilirsiniz. 
    
2. Her biri için kayıt ve çözümleri engelleyen yaygın hataların listesi için bu belgeleri gözden geçirme: Sorun giderme [kılavuzu ve](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) Sorun [giderme belgesi.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [iOS cihazlarını Microsoft Intune'a kaydetmeyi öğrenin.](https://docs.microsoft.com/intune/ios-enroll)
    

