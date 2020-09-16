---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731259"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Intune ile BitLocker şifrelemesini etkinleştirme

 Windows cihazlarında BitLocker şifreleme ayarlarını yapılandırmak için Intune Endpoint Protection Ilkesi kullanılabilir. Daha fazla bilgi için, [Intune kullanarak cihazları korumada Windows 10 (ve sonraki sürümler) ayarlarına](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)bakın.
 
Windows 10 çalıştıran yeni aygıtların, MDM ilkesi uygulaması olmadan tetiklenen otomatik BitLocker şifrelemesini desteklemediğini bilmelisiniz. Bu, varsayılan olmayan ayarlar yapılandırılırsa ilkenin uygulamasını etkileyebilir. Daha ayrıntılı bilgi için aşağıdaki SSS bölümüne bakın.
 
BitLocker sorunlarını giderme hakkında bilgi için [Microsoft Intune 'Da BitLocker Ilkelerinde sorun giderme](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)konusuna bakın.
 
 
**SSS**

 S: Endpoint Protection Ilkesini kullanarak Windows 'un hangi sürümleri cihaz şifrelemesini destekliyor?<br>
 A: Intune Endpoint Protection Ilkesindeki ayarlar [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)kullanılarak uygulanır. Tüm Windows sürümleri veya derlemeleri BitLocker CSP 'yi desteklemez. <br><br>
      Şu anda, aşağıdaki Windows sürümleri desteklenir: Kurumsal, eğitim, mobil, mobil kurumsal ve profesyonel (derleme 1809 ve üstü).
 
S: cihaz zaten şifreleme yöntemi ve şifreleme gücü (XTS-AES-128) için işletim sistemi varsayılan ayarları kullanılarak bir cihaz şifrelenmişse, farklı ayarlarla bir ilke uygulama yeni ayarlarla otomatik olarak yeniden şifrelemeyi tetikleyecektir.<br>
Y: Hayır. Yeni şifre ayarlarını uygulamak için önce sürücünün şifresinin çözülmesi gerekir.<br><br>
**Not:** Autopilot 'e Kaydolmakta olan cihazlar için, Intune ilkesi değerlendirilinceye kadar OOBE sırasında oluşacak Otomatik şifreleme tetiklenemez ve bu da işletim sistemi varsayılanları yerine ilke tabanlı ayarların kullanılmasına olanak tanır.
 
S: Intune ilkesi uygulamasının bir sonucu olarak bir cihaz şifrelenmişse, bu ilke kaldırıldığında şifresi çözülür mi?<br>
A: şifrelemeyle ilgili ilkenin kaldırılması, yapılandırılmış sürücülerin şifresinin çözülmesini sağlamaz.
 
S: Intune uyumluluk Ilkesinde neden aygıtımın BitLocker 'ın etkin olmadığını gösterir, ancak olsa da?<br>
A: Intune uyumluluk Ilkesindeki "BitLocker etkin" ayarı Windows cihaz durumu kanıtlama (DHA) istemcisini kullanır. Bu istemci yalnızca önyükleme sırasında cihaz durumunu ölçtüğünden. Bu nedenle, BitLocker şifrelemesi tamamlandığından bir cihaz yeniden başlatılıncaya kadar, DHA istemci hizmeti BitLocker 'ı etkin olduğu gibi bildirmeyecektir.
 
 