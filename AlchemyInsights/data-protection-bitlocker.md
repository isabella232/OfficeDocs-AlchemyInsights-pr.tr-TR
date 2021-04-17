---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 8166a055d7a967faab83484619b443cc98239c7c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815635"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Intune ile Bitlocker şifrelemesini etkinleştirme

Intune Uç Nokta Koruma İlkesi, Windows cihazları için Bitlocker şifreleme ayarlarını yapılandırmak üzere kullanılabilir. Daha fazla bilgi için, Intune kullanarak cihazları korumak [için Windows 10 (ve sonrası) ayarlarına bakın.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

Uç Nokta Koruma İlkesi'ne ek olarak, cihazlar için şifreleme durumunun daha ayrıntılı bir görünümünü sağlayan bir Şifreleme Raporu da vardır. Bu rapora MEM portalında Cihazlar ve Monitör **altında > ve** sonra Yapılandırma altında Şifreleme [raporu'seçerek erişilebilir.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport) 

Bitlocker'ın beklendiği gibi etkinleştirilmemiş olduğunu veya Bitlocker'ı etkinleştirmek için kullanılan profilin hata durumunda olduğunu fark ederseniz, davranışın neden oluştuğunu daha iyi anlamak için lütfen şifreleme raporunu gözden geçirin.

Raporu çeşitli şifreleme durumu değerleri de içinde olmak üzere nasıl yorumlayacağız hakkında ayrıntılı bilgi için [bkz. Intune ile cihaz şifrelemeyi izleme.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Windows 10 çalıştıran birçok yeni cihaz, MDM ilkesi uygulaması olmadan tetiklenen otomatik Bitlocker şifrelemesini destekler. Varsayılan olmayan ayarlar yapılandırılmışsa bu durum ilke uygulamasını da etkiler. Daha ayrıntılı bilgi için aşağıdaki SSS bölümüne bakın.

Bitlocker sorunlarını giderme hakkında daha fazla bilgi için [bkz. Microsoft Intune'da BitLocker ilkelerini giderme.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**SSS**

S: Uç Nokta Koruma İlkesi kullanılarak Windows desteği cihaz şifrelemenin hangi sürümleri?<br>
Y: Intune Uç Nokta Koruma İlkesi'nin ayarları [Bitlocker CSP kullanılarak uygulanır.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Windows'un tüm sürümleri veya derlemeleri Bitlocker CSP'yi desteklemez. <br><br>

S: Bitlocker son kullanıcı etkileşimi gerektirmeden cihazlarda nasıl etkinleştirilebilir?<br>
A: Gerekli önkulları karşılamız olduğu sürece, Intune aracılığıyla Bitlocker "Sessiz Şifreleme"yi etkinleştirmek mümkündür. Aşağıdaki belgede sessiz şifrelemeyi etkinleştirmek için cihaz gereksinimlerinin ayrıntılarına ve örnek ilke ayarlarına bakın: [BitLocker Şifrelemesi'ni Sessiz Olarak Etkinleştir.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

S: Bir cihaz zaten şifreleme yöntemi ve şifreleme gücü için işletim sistemi varsayılan ayarları (XTS-AES-128) kullanılarak Bitlocker ile şifrelenirse, farklı ayarlara sahip bir ilke uygulama otomatik olarak yeni ayarlarla sürücünün yeniden şifrelenmesini tetikler mi?<br>
Y: Hayır. Yeni şifreleme ayarlarını uygulamak için, önce sürücünün şifresinin çözülmesi gerekir.<br><br>
**Not:** AutoPilot ile kaydolan cihazlar için, Intune ilkesi değerlendirilene kadar OOBE sırasında otomatik şifreleme tetiklanmaz ve bu da işletim sistemi varsayılanları yerine ilke tabanlı ayarların kullanılmalarına olanak tanır.
 
S: Intune ilkesi uygulamasının bir sonucu olarak bir cihaz şifrelenirse, bu ilke kaldırıldığı zaman bu şifre çözülecek mi?<br>
Y: Şifrelemeyle ilgili ilkenin kaldırılması, yapılandırılan sürücülerin şifresinin çözülmesine neden OLMAZ.
 
S: Intune Uyumluluk İlkesi neden cihazımda Bitlocker etkin olmadığını gösteriyor?<br>
A: Intune Uyumluluk İlkesi'nde "Bitlocker etkinleştirildi" ayarı, Windows Cihaz Sistem Durumu Attestation (DHA) istemcisini kullanır. Bu istemci yalnızca cihaz durumunu önyükleme zamanında ölçür. Dolayısıyla, Bitlocker şifrelemesi tamamlandıktan sonra bir cihaz yeniden başlatmamışsa DHA istemci hizmeti Bitlocker'ın etkin olduğunu bildirmez.
 
 