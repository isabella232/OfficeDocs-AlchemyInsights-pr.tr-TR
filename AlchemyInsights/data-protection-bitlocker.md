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
ms.openlocfilehash: 482c08b31e4d97ca5cc9ec6e35e309cb7536036d
ms.sourcegitcommit: 58ac31a58c956a4d74f66bd4151a2311dc361b78
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/07/2021
ms.locfileid: "49778213"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Intune ile BitLocker şifrelemesini etkinleştirme

Windows cihazlarında BitLocker şifreleme ayarlarını yapılandırmak için Intune Endpoint Protection Ilkesi kullanılabilir. Daha fazla bilgi için, [Intune kullanarak cihazları korumada Windows 10 (ve sonraki sürümler) ayarlarına](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)bakın.

Endpoint Protection Ilkesine ek olarak, cihazlar için şifreleme durumunun ayrıntılı görünümünü sağlayan bir şifreleme raporu da vardır. Bu rapora **cihazlar > İzleyicisi** altındaki mem portalından erişilebilir ve sonra **yapılandırma** altında [şifreleme raporu](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)seçin.

BitLocker 'ın beklendiği şekilde etkinleştirilememesini veya BitLocker 'ı etkinleştirmek için kullanılan profilin bir hata durumunda olduğunu fark ederseniz, davranışın neden gerçekleştiğini daha iyi anlamak için lütfen şifreleme raporunu gözden geçirin.

Raporu çeşitli şifreleme durumu değerleriyle birlikte yorumlama hakkında bilgi edinmek için [bkz.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Windows 10 çalıştıran yeni aygıtların, MDM ilkesi uygulaması olmadan tetiklenen otomatik BitLocker şifrelemesini desteklemediğini bilmelisiniz. Bu, varsayılan olmayan ayarlar yapılandırılırsa ilkenin uygulamasını etkileyebilir. Daha ayrıntılı bilgi için aşağıdaki SSS bölümüne bakın.

BitLocker sorunlarını giderme hakkında bilgi için [Microsoft Intune 'Da BitLocker Ilkelerinde sorun giderme](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)konusuna bakın.
 
 
**SSS**

S: Endpoint Protection Ilkesini kullanarak Windows 'un hangi sürümleri cihaz şifrelemesini destekliyor?<br>
A: Intune Endpoint Protection Ilkesindeki ayarlar [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)kullanılarak uygulanır. Tüm Windows sürümleri veya derlemeleri BitLocker CSP 'yi desteklemez. <br><br>

S: Son Kullanıcı etkileşimi gerekmeden cihazlarda BitLocker nasıl etkinleştirilebilir?<br>
A: gerekli önkoşulları karşıladığı için, Intune aracılığıyla BitLocker "sessiz şifrelemeyi" etkinleştirmeniz olasıdır. Aşağıdaki belgede sessiz şifrelemeyi etkinleştirmek için cihaz gereksinimleri ve örnek ilke ayarlarının ayrıntılarına bakın: [BitLocker şifrelemesini sessizce etkinleştirin](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

S: cihaz zaten şifreleme yöntemi ve şifreleme gücü (XTS-AES-128) için işletim sistemi varsayılan ayarları kullanılarak bir cihaz şifrelenmişse, farklı ayarlarla bir ilke uygulama yeni ayarlarla otomatik olarak yeniden şifrelemeyi tetikleyecektir.<br>
Y: Hayır. Yeni şifre ayarlarını uygulamak için önce sürücünün şifresinin çözülmesi gerekir.<br><br>
**Not:** Autopilot 'e Kaydolmakta olan cihazlar için, Intune ilkesi değerlendirilinceye kadar OOBE sırasında oluşacak Otomatik şifreleme tetiklenemez ve bu da işletim sistemi varsayılanları yerine ilke tabanlı ayarların kullanılmasına olanak tanır.
 
S: Intune ilkesi uygulamasının bir sonucu olarak bir cihaz şifrelenmişse, bu ilke kaldırıldığında şifresi çözülür mi?<br>
A: şifrelemeyle ilgili ilkenin kaldırılması, yapılandırılmış sürücülerin şifresinin çözülmesini sağlamaz.
 
S: Intune uyumluluk Ilkesinde neden aygıtımın BitLocker 'ın etkin olmadığını gösterir, ancak olsa da?<br>
A: Intune uyumluluk Ilkesindeki "BitLocker etkin" ayarı Windows cihaz durumu kanıtlama (DHA) istemcisini kullanır. Bu istemci yalnızca önyükleme sırasında cihaz durumunu ölçtüğünden. Bu nedenle, BitLocker şifrelemesi tamamlandığından bir cihaz yeniden başlatılıncaya kadar, DHA istemci hizmeti BitLocker 'ı etkin olduğu gibi bildirmeyecektir.
 
 