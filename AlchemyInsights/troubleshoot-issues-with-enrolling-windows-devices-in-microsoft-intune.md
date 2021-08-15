---
title: Microsoft Intune'da Windows cihazlarını kaydetmeyle ilgili sorunları Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981061"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Microsoft Intune'da Windows cihazlarını kaydetmeyle ilgili sorunları Microsoft Intune

Sorununuzu çözmek için aşağıda listelenen kaynakları gözden geçirebilirsiniz.
  
Sık karşılaşılan bazı hata iletileri ve çözüm adımları:
  
 **Yazılım yük olamaz, 0x80cf4017:** Hesap sertifikanın süresi doldu. Intune Yönetim Konsolu'nu kullanarak BILGISAYAR İstemcisi yazılım paketini yeniden indirin. Daha fazla bilgi için bu belgeleri gözden geçirebilirsiniz.
  
 **Hata kodu 0x801c0003:** Hata aşağıdaki senaryolarda oluşabilir:
  
-  Kullanıcının cihaz sınırının üzerinde kayıtlı cihazı var. Cihazı kaldırmak veya [cihaz sınırını değiştirmek için](https://docs.microsoft.com/intune/devices-wipe) bu belgeleri gözden [geçirebilirsiniz.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Kullanıcılar Azure AD'ye cihazlara katılabilir" olarak "yok" ayarlanır. Tüm kullanıcılara ayarlayın veya kullanıcıları seçin. Daha [fazla bilgi için bu](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) belgeleri gözden geçirebilirsiniz.

-  Cihaz başka bir kullanıcı tarafından zaten kayıtlı. Böyle bir durumda, yeniden çalışmadan önce cihazı Azure Intune konsolundan kaldırın veya el ile kaydı kaldırın.

-  Cihaz şu Windows 10 Home. Yalnızca Windows 10 Pro, Eğitim ve Enterprise SKUs tarafından Azure Active Directory.

Sorununuzu çözmenize yardımcı olacak ek kaynaklar:
  
-  Yaygın kayıt sorunlarını tanılamak ve gidermek için [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) Sorun Giderme Portalı'nın kullanın. Daha [fazla ayrıntı için](https://docs.microsoft.com/intune/help-desk-operators) bu belgeyi gözden geçirebilirsiniz.

-  Kayıt ve çözümleri engelleyen yaygın hataların listesi için bu belgeleri gözden geçirebilirsiniz: Sorun giderme [kılavuzu](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ve [Sorun giderme belgesi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Microsoft Intune'da Windows cihazları nasıl Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
