---
title: Windows aygıtlarını Microsoft Intune'a kaydetme yle ilgili sorun giderme sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665852"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Windows aygıtlarını Microsoft Intune'a kaydetme yle ilgili sorun giderme sorunları

Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirin.
  
Bazı yaygın hata iletileri ve çözüm adımları:
  
 **Yazılım, 0x80cf4017 yüklenemez:** Hesap sertifikanızın süresi doldu. PC Client yazılım paketini Intune Admin Konsoluna yeniden indirin. Daha fazla bilgi için bu belgeleri gözden geçirin.
  
 **Hata kodu 0x801c0003:** Hata aşağıdaki senaryolarda oluşabilir:
  
-  Kullanıcı, aygıt sınırından daha fazla aygıt alabilenir. [Aygıtı kaldırmak](https://docs.microsoft.com/intune/devices-wipe) veya aygıt [sınırını değiştirmek](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)için bu belgeleri gözden geçirin.

-  "Kullanıcılar aygıtları Azure AD'ye katılabilir" olarak ayarlanır". Tüm ünü veya belirli kullanıcılara ayarlayın. Daha fazla bilgi için [bu belgeleri](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) gözden geçirin.

-  Aygıt zaten başka bir kullanıcı tarafından kaydedilen. Bu durumda, yeniden denemeden önce aygıtı Azure Intune konsolundan çıkarın veya aygıtı el ile kaldırın.

-  Cihaz Windows 10 Home'dur. Azure Active Directory'ye yalnızca Windows 10 Pro, Eğitim ve Kurumsal SK'ler katılabilir.

Sorununuzu çözmeye yardımcı olacak ek kaynaklar:
  
-  Sık karşılaşılan kayıt hatalarını tanılamak ve gidermek için [Intune Sorun Giderme Portalı'nı](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) kullanın. Daha fazla ayrıntı için [bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) gözden geçirin.

-  Bu belgeleri, her birine kaydolmasını ve çözümlerini engelleyen yaygın hataların bir listesi için gözden geçirin: [Sorun Giderme kılavuzu](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ve [Sorun Giderme dokümanı.](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)

[Windows aygıtlarını Microsoft Intune'a nasıl kaydedebilirsiniz öğrenin.](https://docs.microsoft.com/intune/windows-enroll)
