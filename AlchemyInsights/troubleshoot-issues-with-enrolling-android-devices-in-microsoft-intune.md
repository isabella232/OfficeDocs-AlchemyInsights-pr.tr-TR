---
title: Microsoft Intune'da Android cihazlarını kaydetmeyle ilgili sorunları giderme
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830962"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Microsoft Intune'da Android cihazlarını kaydetmeyle ilgili sorunları giderme

Sorununuzu çözmek için aşağıda listelenen kaynakları gözden geçirebilirsiniz.
  
Sık karşılaşılan bazı sorunlar ve çözüm adımları:
  
 **Şirket Portalında Şifrelenmiş Değil hatası:** Özellikle v7.0 ile başlayan yeni Android sürümleri, cihazınızın tümüyle şifre olduğundan emin olmak için bir başlangıç geçiş kodu gerektirir. Yaygın çözümler, bir başlangıç PIN'ini etkinleştirmek veya cihazı tam olarak şifrelemektir. Daha [fazla bilgi için](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) bu belgeyi gözden geçirebilirsiniz.
  
 **Cihazlar Intune hizmetiyle iade başarısız olur veya Intune** yönetim konsolunda "Sağlıksız" olarak görüntülenir: Bazı Samsung 4.4 ve 5.5 cihazları hizmeti kontrol edeyemmektedir. Bu sorunun 3 olası çözümü vardır:
  
1. Cihaz eşitlemeyi otomatik olarak başlatan Intune Şirket Portalı uygulamasını el ile açın.

2. Cihazı Android 6.0 veya daha yeni bir sürümüne güncelleştirin.

3. Samsung Smart Manager'ın Intune Şirket Portalı'ni yönetmesini devre dışı bırak. Bu [sorunlar ve](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) çözümle ilgili daha ayrıntılı bilgi için bu belgeyi gözden geçirebilirsiniz.

 **Kullanıcı Lisans Türü Geçersiz** **veya Kullanıcı Adı Tanınmadı hatası:** Kullanıcıya Intune veya EMS lisansı atanıyor olması gerekir. Lisans atamak için şu belgeleri gözden geçirebilirsiniz: Office Yönetim Merkezi veya Azure portalı.
  
Sorununuzu çözmenize yardımcı olacak ek kaynaklar:
  
1. Yaygın kayıt sorunlarını tanılamak ve gidermek için [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) Sorun Giderme Portalı'nın kullanın. Daha [fazla ayrıntı için](https://docs.microsoft.com/intune/help-desk-operators) bu belgeyi gözden geçirebilirsiniz.

2. Kayıt [ve çözümlerini](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) engelleyen yaygın hataların listesi için bu belgeyi gözden geçirebilirsiniz.

3. [Android cihazları Microsoft Intune'a nasıl kaydeden öğrenin.](https://docs.microsoft.com/intune/android-enroll)
