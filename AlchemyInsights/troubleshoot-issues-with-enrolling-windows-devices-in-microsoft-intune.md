---
title: Kaydolma Microsoft Intune aygıtlar Windows ile sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28318325"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Kaydolma Microsoft Intune aygıtlar Windows ile sorunlarını giderme

Şimdi, sorunu gidermek için aşağıda listelenen kaynakları inceleyin. 
  
Bazı yaygın hata iletileri ve çözümleme adımları:
  
 **Yazılımı yüklenemiyor, 0x80cf4017:** Hesap sertifikanızın süresi dolmuş. Intune yönetim konsolunda PC istemci yazılım paketini yeniden yükleyin. Daha fazla bilgi için bu belge gözden geçirin. 
  
 **0x801c0003 hata kodu:** Hata aşağıdaki senaryolarda ortaya çıkabilir: 
  
1. Daha fazla aygıtlar Aygıt üst sınırından kayıtlı kullanıcı vardır. [Bir aygıtı kaldırmak](https://docs.microsoft.com/en-us/intune/devices-wipe) veya [aygıt bu sınırı değiştirmek](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions)için bu belgeleri gözden geçirin.
    
2. "Kullanıcıların aygıtlar için Azure AD katılabilirsiniz" "yok" olarak ayarlanır. Tümüne ayarlayın veya seçin kullanıcılar. Daha fazla bilgi için [Bu belge](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) gözden geçirin. 
    
3. Aygıt zaten başka bir kullanıcı tarafından kaydedilmiş. Bu durumda, aygıt Azure Intune konsoldan kaldırmak veya yeniden denemeden önce aygıtı el ile unenroll.
    
4. Windows 10 giriş aygıtıdır. Azure Active Directory, yalnızca Windows 10 Pro, eğitim ve Kurumsal SKU'ları katılabilirsiniz.
    
Sorununuzu gidermeye yardımcı olmak için ek kaynaklar:
  
1. [Intune sorun giderme Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) tanılamak ve ortak kayıt hatalarını gidermek için kullanın. Daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/en-us/intune/help-desk-operators) gözden geçirin. 
    
2. Bu belgeler için kayıt ve çözümler için her önlemek sık karşılaşılan hataların listesini gözden geçirin: [sorun giderme kılavuzu](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ve [sorun giderme doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Microsoft Intune Windows aygıtları kaydetmek öğrenin](https://docs.microsoft.com/en-us/intune/windows-enroll).
  

