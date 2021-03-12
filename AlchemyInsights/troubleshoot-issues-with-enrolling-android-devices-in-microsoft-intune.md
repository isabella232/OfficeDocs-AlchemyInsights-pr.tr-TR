---
title: Microsoft Intune'da Android cihazlarını kaydetmeyle ilgili sorunları giderme
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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709018"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Microsoft Intune'da Android cihazlarını kaydetmeyle ilgili sorunları giderme

Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirebilirsiniz.
  
Sık karşılaşılan bazı sorunlar ve çözüm adımları:
  
 **Şirket Portalında Cihaz Şifreli değil hatası:** Özellikle v7.0 ile başlayan daha yeni Android sürümleri, cihazınızın tamamen şifrelenmiş olduğundan emin olmak için başlangıç geçiş kodu gerektirir. Yaygın çözümler, bir başlangıç pin'ini etkinleştirmek veya cihazı tamamen şifrelemektir. Daha [fazla bilgi için](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) bu belgeyi gözden geçirebilirsiniz.
  
 **Cihazlar Intune hizmetiyle iade başarısız oluyor veya Intune yönetici konsolunda "Sağlıksız" olarak görüntüleniyor:** Bazı Samsung 4.4 ve 5.5 cihazları hizmette yer alamayyabilirsiniz. Bu sorunun 3 olası çözümü vardır:
  
1. Cihaz eşitlemeyi otomatik olarak başlatan Intune Şirket Portalı uygulamasını el ile açın.

2. Cihazı Android 6.0 veya daha yeni bir sürümüne güncelleştirin.

3. Samsung Smart Manager'ın Intune Şirket Portalı'nın yönetiminden devre dışı bırakma. Bu [sorunlar ve](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) çözümle ilgili daha ayrıntılı bilgi için bu belgeyi gözden geçirebilirsiniz.

 **Kullanıcı Lisans Türü Geçersiz** veya **Kullanıcı Adı Tanınmadı hatası:** Kullanıcıya Intune veya EMS lisansı atanıyor olması gerekir. Şu belgeleri gözden geçirerek lisans atabilirsiniz: Office Yönetim Merkezi veya Azure portalı.
  
Sorununuzu çözmenize yardımcı olacak ek kaynaklar:
  
1. Yaygın [kayıt hatalarını tanılamak ve](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) çözmek için Intune Sorun Giderme Portalı'nın kullanın. Daha [fazla ayrıntı için](https://docs.microsoft.com/intune/help-desk-operators) bu belgeyi gözden geçirebilirsiniz.

2. Her [biri için](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) kayıt ve çözüm engelleyen yaygın hataların listesi için bu belgeyi gözden geçirebilirsiniz.

3. [Android cihazlarını Microsoft Intune'a kaydetmeyi öğrenin.](https://docs.microsoft.com/intune/android-enroll)
