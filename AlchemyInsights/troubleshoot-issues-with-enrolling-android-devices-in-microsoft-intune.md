---
title: Microsoft Intune Android aygıtlar kaydolma sorunları giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655903"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Microsoft Intune Android aygıtlar kaydolma sorunları giderme

Şimdi, sorunu gidermek için aşağıda listelenen kaynakları inceleyin.
  
Bazı sık karşılaşılan sorunlar ve çözüm adımları:
  
 **Aygıt şifreli şirket Portal hatası:** Android, özellikle v7.0 ile başlayan yeni sürümleri, aygıt tam olarak şifrelendiğinden emin olmak için bir başlangıç parolası gerektirir. Başlangıç PIN'i etkinleştirmek veya aygıt tam olarak şifrelemek için ortak çözümler şunlardır. Daha fazla bilgi için [Bu belgeyi](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) gözden geçirin. 
  
 **Aygıtları başarısız Intune hizmeti ile denetlemek veya Intune yönetim konsolunda "Sağlıksız" görüntülemek:** Bazı Samsung 4.4 ve 5.5 aygıtları hizmette oturum denetimi yapamayabilirsiniz. Bu sorundan 3 olası çözümler şunlardır: 
  
1. Otomatik olarak bir aygıt eşitleme başlatacağı Intune şirket Portal uygulamayı el ile açın.
    
2. Android 6.0 veya daha fazla aygıt güncelleştirin.
    
3. Samsung akıllı Yöneticisi dan Intune şirket Portal Yönetimi devre dışı bırakın. Bu sorunlar ve çözümleri hakkında daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) gözden geçirin. 
    
 **Kullanıcı lisans türü geçersiz** veya **kullanıcı adı tanınmadı hatası:** kullanıcı Intune veya EMS bir lisans atanması gerekir. Bir lisans aracılığıyla atamak için bu belgeleri gözden geçirin: Office Yönetim Merkezi veya Azure portal. 
  
Sorununuzu gidermeye yardımcı olmak için ek kaynaklar:
  
1. [Intune sorun giderme Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) tanılamak ve ortak kayıt hatalarını gidermek için kullanın. Daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) gözden geçirin. 
    
2. [Bu belge](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) için kayıt ve çözümler için her önlemek sık karşılaşılan hataların listesini gözden geçirin. 
    
3. [Microsoft Intune Android aygıtlar kaydetmeyi öğrenin](https://docs.microsoft.com/intune/android-enroll).
    

