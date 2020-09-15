---
title: Microsoft Intune 'da Android cihazlarını kaydetme sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689974"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Microsoft Intune 'da Android cihazlarını kaydetme sorunlarını giderme

Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirin.
  
Bazı yaygın sorunlar ve çözüm adımları:
  
 **Şirket portalında cihaz şifrelenmemiş hatası:** Cihazınızın tümüyle şifrelendiğinden emin olmak için, özellikle de v 7.0 ile başlayan Android 'in daha yeni sürümleri için başlangıç parolası gerekir. Genel çözümler, başlangıç PIN 'ini etkinleştirmek veya cihazı tümüyle şifrelemektir. Daha fazla bilgi için [Bu belgeyi](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) gözden geçirin.
  
 **Cihazlar Intune hizmetine iade edemeyecek veya Intune yönetim konsolunda "sağlıksız" olarak görüntülenmeyecek:** Bazı Samsung 4,4 ve 5,5 cihazları hizmeti iade edebilir. Bu sorunun 3 olası çözümü vardır:
  
1. Cihaz eşitlemesini otomatik olarak başlatan Intune şirket portalı uygulamasını el ile açın.

2. Cihazı Android 6,0 veya üzeri olarak güncelleyin.

3. Samsung akıllı Manager 'ın Intune şirket portalını yönetmesini devre dışı bırakın. Bu sorunlar ve çözünürlükler hakkında daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) inceleyin.

 **Kullanıcı Lisans türü geçersiz** veya **Kullanıcı adı tanınmadı hata:** kullanıcıya bir Intune veya EMS lisansı atanmalıdır. Office Yönetim Merkezi veya Azure Portal aracılığıyla lisans atamak için bu belgeleri gözden geçirin.
  
Sorununuzu çözmek için ek kaynaklar:
  
1. Yaygın kayıt hatalarını tanılamak ve çözmek için [Intune sorun giderme portalı](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 'nı kullanın. Daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) inceleyin.

2. Her biri için kayıt ve çözünürlüğe engel olan yaygın hataların listesi için [Bu belgeyi](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) inceleyin.

3. [Android cihazlarını Microsoft Intune 'da kaydettirme hakkında bilgi edinin](https://docs.microsoft.com/intune/android-enroll).
