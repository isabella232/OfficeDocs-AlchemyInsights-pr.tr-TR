---
title: Windows cihazlarını Microsoft Intune'a kaydetmeyle ilgili sorunları giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708910"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Windows cihazlarını Microsoft Intune'a kaydetmeyle ilgili sorunları giderme

Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirebilirsiniz.
  
Sık karşılaşılan bazı hata iletileri ve çözüm adımları:
  
 **Yazılım yük olamaz, 0x80cf4017:** Hesap sertifikanın süresi doldu. Intune Yönetim Konsolu'nu kullanarak BILGISAYAR İstemcisi yazılım paketini yeniden indirin. Daha fazla bilgi için bu belgeleri gözden geçirebilirsiniz.
  
 **Hata kodu 0x801c0003:** Hata aşağıdaki senaryolarda oluşabilir:
  
-  Kullanıcının cihaz sınırının üzerinde kayıtlı cihazı var. Bir cihazı kaldırmak veya [cihaz sınırını değiştirmek](https://docs.microsoft.com/intune/devices-wipe) için bu belgeleri gözden [geçirebilirsiniz.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Kullanıcılar cihazları Azure AD'ye katılabilir" olarak "yok" olarak ayarlanır. Bunu tüm kullanıcılara veya belirli kullanıcılara ayarlayın. Daha [fazla bilgi için bu](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) belgeleri gözden geçirebilirsiniz.

-  Cihaz zaten başka bir kullanıcı tarafından kayıtlı. Böyle bir durumda, cihazı Azure Intune konsolundan kaldırın veya yeniden deneyin.

-  Cihaz Windows 10 Home'tır. Azure Active Directory'ye yalnızca Windows 10 Pro, Eğitim ve Kurumsal SKUs katılabilir.

Sorununuzu çözmenize yardımcı olacak ek kaynaklar:
  
-  Yaygın [kayıt hatalarını tanılamak ve](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) çözmek için Intune Sorun Giderme Portalı'nın kullanın. Daha [fazla ayrıntı için](https://docs.microsoft.com/intune/help-desk-operators) bu belgeyi gözden geçirebilirsiniz.

-  Her biri için kayıt ve çözümleri engelleyen yaygın hataların listesi için bu belgeleri gözden geçirme: Sorun giderme [kılavuzu ve](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) Sorun [giderme belgesi.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Windows cihazlarını Microsoft Intune'a kaydetmeyi öğrenin.](https://docs.microsoft.com/intune/windows-enroll)
