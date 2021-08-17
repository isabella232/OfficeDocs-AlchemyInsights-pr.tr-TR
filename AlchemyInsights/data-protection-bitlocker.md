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
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118620"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Intune ile Bitlocker şifrelemesini etkinleştirme

Intune Endpoint Protection İlkesi, diğer cihazlar için Bitlocker şifreleme ayarlarını yapılandırmak Windows kullanılabilir. Daha fazla bilgi için [bkz. Intune Windows 10](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)cihazları korumak için güvenlik (ve sonrası) ayarlarını değiştirme .

Şifreleme İlkesi'Endpoint Protection yanı sıra, cihazlar için şifreleme durumunun daha ayrıntılı bir görünümünü sağlayan bir Şifreleme Raporu da vardır. Bu rapora MEM portalında Cihazlar ve Monitör **altında > ve** sonra Yapılandırma altında Şifreleme [raporu'seçerek erişilebilir.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport) 

Bitlocker'ın beklendiği gibi etkinleştirilmemiş olduğunu veya Bitlocker'ı etkinleştirmek için kullanılan profilin hata durumunda olduğunu fark ederseniz, davranışın neden oluştuğunu daha iyi anlamak için lütfen şifreleme raporunu gözden geçirin.

Raporu çeşitli şifreleme durumu değerleri de içinde olmak üzere nasıl yorumlayacağız hakkında ayrıntılı bilgi için [bkz. Intune ile cihaz şifrelemeyi izleme.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Daha yeni olan birçok cihaz, Windows 10 MDM ilkesi uygulaması olmadan tetiklenen otomatik Bitlocker şifrelemeyi destekler. Varsayılan olmayan ayarlar yapılandırılmışsa bu durum ilke uygulamasını da etkiler. Daha ayrıntılı bilgi için aşağıdaki SSS bölümüne bakın.

Bitlocker sorunlarını giderme hakkında daha fazla bilgi için [bkz. BitLocker ilkeleriyle ilgili sorunları giderme Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**SSS**

S: İlke İlkesi'Windows desteklenen cihaz şifrelemenin Endpoint Protection var?<br>
Y: Intune Genel Endpoint Protection ayarları [Bitlocker CSP kullanılarak uygulanır.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Bitlocker CSP'nin tüm sürümleri Windows sürümleri veya derlemeleri desteklemez. <br><br>

S: Bitlocker son kullanıcı etkileşimi gerektirmeden cihazlarda nasıl etkinleştirilebilir?<br>
A: Gerekli önkulları karşılamız olduğu sürece, Intune aracılığıyla Bitlocker "Sessiz Şifreleme"yi etkinleştirmek mümkündür. Aşağıdaki belgede sessiz şifrelemeyi etkinleştirmek için cihaz gereksinimlerinin ayrıntılarına ve örnek ilke ayarlarına bakın: [BitLocker Şifrelemesi'ni Sessiz Olarak Etkinleştir.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

S: Bir cihaz zaten şifreleme yöntemi ve şifreleme gücü için işletim sistemi varsayılan ayarları (XTS-AES-128) kullanılarak Bitlocker ile şifrelenirse, farklı ayarlara sahip bir ilke uygulama otomatik olarak yeni ayarlarla sürücünün yeniden şifrelenmesini tetikler mi?<br>
C: Hayır. Yeni şifreleme ayarlarını uygulamak için, önce sürücünün şifresinin çözülmesi gerekir.<br><br>
**Not:** AutoPilot ile kaydolan cihazlar için, Intune ilkesi değerlendirilene kadar OOBE sırasında otomatik şifreleme tetiklanmaz ve bu da işletim sistemi varsayılanları yerine ilke tabanlı ayarların kullanılmalarına olanak tanır.
 
S: Intune ilkesi uygulamasının bir sonucu olarak bir cihaz şifrelenirse, bu ilke kaldırıldığı zaman bu şifre çözülecek mi?<br>
Y: Şifrelemeyle ilgili ilkenin kaldırılması, yapılandırılan sürücülerin şifresinin çözülmesine neden OLMAZ.
 
S: Intune Uyumluluk İlkesi neden cihazımda Bitlocker etkin olmadığını gösteriyor?<br>
A: Intune Uyumluluk İlkesi'nde "Bitlocker etkinleştirildi" ayarı, Cihaz Windows (DHA) istemcisini kullanır. Bu istemci yalnızca cihaz durumunu önyükleme zamanında ölçür. Dolayısıyla, Bitlocker şifrelemesi tamamlandıktan sonra bir cihaz yeniden başlatmamışsa DHA istemci hizmeti Bitlocker'ın etkin olduğunu bildirmez.
 
 