---
title: Android cihazlarımicrosoft Intune'a kaydetme yle ilgili sorun giderme sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759640"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Android cihazlarımicrosoft Intune'a kaydetme yle ilgili sorun giderme sorunları

Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirin.
  
Bazı sık karşılaşılan sorunlar ve çözüm adımları:
  
 **Şirket Portalında Şifrelenmemiş Aygıt Hatası:** Android'in özellikle v7.0 ile başlayan yeni sürümleri, cihazınızın tamamen şifrelenmiş olduğundan emin olmak için bir başlangıç şifresi gerektirir. Ortak çözümler bir başlangıç pin etkinleştirmek veya tamamen aygıtı şifrelemek içinvardır. Daha fazla bilgi için [bu belgeyi](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) gözden geçirin.
  
 **Aygıtlar Intune hizmetiyle check-in yapmayı veya Intune yönetici konsolunda "Sağlıksız" olarak görüntülenememektedir:** Bazı Samsung 4.4 ve 5.5 cihazları hizmete giriş olmayabilir. Bu sorunun 3 olası çözümü vardır:
  
1. Bir aygıt senkronizasyonuna otomatik olarak başlayacak olan Intune Company Portal uygulamasını el ile açın.

2. Cihazı Android 6.0 veya üzeri olarak güncelleyin.

3. Samsung Smart Manager'ı Intune Company Portalını yönetmekten devre dışı edin. Bu sorunlar ve çözümler hakkında daha fazla bilgi için [bu belgeyi](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) gözden geçirin.

 **Kullanıcı Lisans Türü Geçersiz** veya **Kullanıcı Adı Tanınmayan hata:** Kullanıcıya bir Intune veya EMS lisansı atanması gerekir. Aşağıdakiler üzerinden lisans atamak için bu belgeleri gözden geçirin: Office Yönetici Merkezi veya Azure portalı.
  
Sorununuzu çözmeye yardımcı olacak ek kaynaklar:
  
1. Sık karşılaşılan kayıt hatalarını tanılamak ve gidermek için [Intune Sorun Giderme Portalı'nı](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) kullanın. Daha fazla ayrıntı için [bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) gözden geçirin.

2. Her biri için kayıt ve çözümleri engelleyen yaygın hataların bir listesi için [bu belgeyi](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) gözden geçirin.

3. [Android aygıtları Microsoft Intune'a nasıl kaydedebilirsiniz öğrenin.](https://docs.microsoft.com/intune/android-enroll)
