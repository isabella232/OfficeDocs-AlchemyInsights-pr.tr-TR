---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908729"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Intune ile Bitlocker şifrelemesini etkinleştirme

 Intune Endpoint Protection Policy, Windows aygıtları için Bitlocker şifreleme ayarlarını yapılandırmak için kullanılabilir. Daha fazla bilgi için, [Intune kullanan aygıtları korumak için Windows 10 (ve sonraki) ayarlarına](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)bakın.
 
Windows 10 çalıştıran birçok yeni aygıtın MDM ilkesi uygulanmadan tetiklenen otomatik Bitlocker şifrelemesini desteklediğini unutmayın. Varsayılan olmayan ayarlar yapılandırılırsa, bu ilkenin uygulanmasını etkileyebilir. Daha fazla ayrıntı için aşağıdaki SSS bölümüne bakın.
 
Bitlocker sorun giderme sorunları hakkında daha fazla bilgi için [Microsoft Intune'daki Sorun Giderme BitLocker ilkelerine](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)bakın.
 
 
**SSS**

 S: Endpoint Protection İlkesi'ni kullanarak Windows destek aygıt şifrelemesinin hangi sürümleri?<br>
 C: Intune Endpoint Protection Policy'deki ayarlar [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)kullanılarak uygulanır. Windows'un tüm sürümleri veya yapıları Bitlocker CSP'yi desteklemez. <br><br>
      Şu anda aşağıdaki Windows sürümleri desteklenir: Enterprise, Education, Mobile, Mobile Enterprise ve Professional (1809 ve sonrası oluşturun).
 
S: Bir aygıt şifreleme yöntemi ve şifreleme gücü (XTS-AES-128) için işletim sistemi varsayılan ayarlarını kullanarak Bitlocker ile zaten şifrelenmişse, farklı ayarlara sahip bir ilke uygulamak sürücünün yeni ayarlarla otomatik olarak yeniden şifrelemesini tetikler mi?<br>
C: Hayır. Yeni şifreleme ayarlarını uygulamak için önce sürücünün şifresinin çözülmesi gerekir.<br><br>
**Not:** Otomatik Pilot'a kaydolan aygıtlar için, INtune ilkesi değerlendirilene kadar OOBE sırasında oluşacak otomatik şifreleme tetiklenmez ve bu da işletim sistemi varsayılanları yerine ilke tabanlı ayarların kullanılmasına olanak tanır.
 
S: Bir aygıt Intune ilkesinin uygulanması sonucunda şifrelenirse, bu ilke kaldırıldığında şifresi çözülür mü?<br>
C: Şifrelemeyle ilgili ilkekaldırılması, yapılandırılan sürücülerin şifresinin çözülmesiyle sonuçlanmaz.
 
S: Intune Uyumluluk İlkesi, aygıtımda bitlocker etkin olmadığını neden gösteriyor?<br>
C: Intune Uyumluluk İlkesi'ndeki "Bitlocker etkin" ayarı, Windows Aygıt Durumu Attestation (DHA) istemcisini kullanır. Bu istemci yalnızca önyükleme zamanında aygıt durumunu ölçer. Bu nedenle, Bitlocker şifrelemesi tamamlandığından beri bir aygıt yeniden başlatılmazsa, DHA istemci hizmeti Bitlocker'ı etkin olarak bildirmez.
 
 