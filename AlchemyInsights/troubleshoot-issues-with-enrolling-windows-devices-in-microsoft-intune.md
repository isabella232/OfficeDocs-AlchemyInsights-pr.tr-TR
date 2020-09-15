---
title: Microsoft Intune 'da Windows cihazlarını kaydetme sorunlarını giderme
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
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658898"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Microsoft Intune 'da Windows cihazlarını kaydetme sorunlarını giderme

Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirin.
  
Bazı yaygın hata iletileri ve çözüm adımları:
  
 **Yazılım yüklenemiyor, 0x80cf4017:** Hesap sertifikanızın süresi doldu. Intune yönetim konsolundaki PC Istemcisi yazılımı paketini yeniden indirin. Daha fazla bilgi için bu belgeyi inceleyin.
  
 **Hata kodu 0x801c0003:** Hata aşağıdaki senaryolarda oluşabilir:
  
-  Kullanıcının cihaz sınırından daha fazla kayıtlı cihazı var. [Cihazı kaldırmak](https://docs.microsoft.com/intune/devices-wipe) veya [cihaz sınırını değiştirmek](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)için bu belgeleri gözden geçirin.

-  "Kullanıcılar cihazları Azure AD 'ye katılabilir" "yok" olarak ayarlanır. Tümünü ayarlayın veya kullanıcıları seçin. Daha fazla bilgi için [Bu belgeyi](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) inceleyin.

-  Cihaz zaten başka bir kullanıcı tarafından kaydedilmiş. Bu durumda, cihazı Azure Intune konsolundan kaldırın veya yeniden denemeden önce cihazı el ile kaldırın.

-  Cihaz Windows 10 ev. Yalnızca Windows 10 Pro, eğitim ve kurumsal SKU 'Lar Azure Active Directory 'ye katılabilir.

Sorununuzu çözmek için ek kaynaklar:
  
-  Yaygın kayıt hatalarını tanılamak ve çözmek için [Intune sorun giderme portalı](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 'nı kullanın. Daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) inceleyin.

-  Her biri için kayıt ve çözünürlüğe engel olan yaygın hataların listesi için bu belgeleri gözden geçirin: [sorun giderme kılavuzu](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ve [belge sorunlarını giderme](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)

[Microsoft Intune 'Da Windows cihazlarını kaydettirme hakkında bilgi edinin](https://docs.microsoft.com/intune/windows-enroll).
