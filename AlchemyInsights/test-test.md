---
title: SharePoint Online Terim Deposu'SharePoint koşulların eksik olduğu koşullar
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106452"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Intune ile BitLocker Şifrelemesini Etkinleştirme

Intune Endpoint Protection İlkesi, şu şekilde açıklandığı gibi Windows cihazları için Boitlocker şifreleme ayarlarını yapılandırmak üzere kullanılabilir: Intune kullanarak cihazları korumak için Windows10 (ve sonrası) ayarları

MDM ilkesi uygulaması olmadan tetiklenen Windows 10 bitlocker şifrelemesi destekleyen daha yeni birçok cihaz olduğunu biliyor olun. Varsayılan olmayan ayarlar yapılandırılmışsa, bu durum ilke uygulamasını da etkileyebilir. Daha ayrıntılı bilgi için bkz. SSS.


S: İlke İlkesi'Windows desteklenen cihaz şifrelemenin hangi Endpoint Protection?
Y: Intune Genel Endpoint Protection ayarları Bitlocker CSP kullanılarak uygulanır.  Bitlocker CSP'nin tüm sürümleri Windows sürümleri veya derlemeleri desteklemez. Şu anda Windows Sürümleri: Enterprise; Eğitim, Mobil, Enterprise Professional (derleme 1809'dan itibaren) desteklemektedir.




S: Bir cihaz zaten şifreleme yöntemi ve şifreleme gücü için işletim sistemi varsayılan ayarları (XTS-AES-128) kullanılarak Bitlocker ile şifrelenirse, farklı ayarlara sahip bir ilke uygulama otomatik olarak yeni ayarlarla sürücü yeniden şifrelenir mi?

C: Hayır. Yeni şifreleme ayarlarını uygulamak için önce sürücünün şifresinin çözülmüş olması gerekir.

Not AutoPilot ile kaydolan cihazlar için, Intune ilkesi değerlendirilinceye kadar OOBE sırasında otomatik şifreleme tetiklanmaz ve bu da işletim sistemi varsayılanları yerine ilke tabanlı ayarların kullanılmalarına olanak tanır




S Intune ilkesi uygulamasının bir sonucu olarak bir cihaz şifrelenirse, bu ilke kaldırıldığı zaman bu cihazın şifresi çözülecektir mi?

Y: Şifrelemeyle ilgili ilkenin kaldırılması, yapılandırılan sürücülerin şifre çözme işlemiYLE sonuçlanmaz.




S: Intune Uyumluluk ilkesi neden cihazımda "Bitlocker Etkin" olmadığını gösteriyor ama etkin?

A: Intune uyumluluk ilkesinde "Bitlocker etkin" ayarı, cihaz sistem Windows (DHA) istemcisini kullanır. Bu istemci yalnızca cihaz durumunu önyükleme zamanında ölçür. Dolayısıyla bitlocker şifrelemesi tamamlandıktan sonra bir cihaz yeniden başlatlanmadısa DHA istemci hizmeti bitlocker'ın etkin olduğunu bildirmez.