---
title: SharePoint Online Term Store'dan eksik terimler
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766873"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Intune ile Bitlocker Şifrelemesini Etkinleştirme

Intune Endpoint Protection Policy, Windows aygıtları için Boitlocker şifreleme ayarlarını açıklandığı gibi yapılandırmak için kullanılabilir: Windows10 (ve sonraki) ayarlarını Intune kullanan aygıtları korumak için

Windows 10 çalıştıran birçok yeni aygıtın MDM ilkesi uygulaması olmadan tetiklenen otomatik bitlocker şifrelemesini desteklediğini unutmayın. Varsayılan olmayan ayarlar yapılandırılırsa, bu ilkenin uygulanmasını etkileyebilir. Daha fazla ayrıntı için SSS bölümüne bakın.


 SSS S: Son Nokta Koruma İlkesi'ni kullanarak Windows'un aygıt şifrelemesini destekleyen sürümleri?
 C: Intune Endpoint Protection Policy'deki ayarlar Bitlocker CSP kullanılarak uygulanır.Tüm sürümleri veya Windows yapıları Bitlocker CSP'yi desteklemez. 
      Şu anda Windows Editions: Enterprise; Eğitim, Mobil, Mobil Kurumsal ve Profesyonel (1809'dan itibaren) desteklenir.




S: Bir aygıt şifreleme yöntemi ve şifreleme gücü (XTS-AES-128) için işletim sistemi varsayılan ayarlarını kullanarak Bitlocker ile zaten şifrelenmişse, farklı ayarlara sahip bir ilke uygulayacak sayılsa, yeni ayarlarla sürücünün yeniden şifrelemesini otomatik olarak tetikler mi?

C: Hayır. Yeni şifreleme ayarlarını uygulamak için öncelikle sürücünün şifresinin çözülmesi gerekir.

Not Otomatik Pilot'a kayıtlı olan aygıtlar için, INtune ilkesi değerlendirilene kadar OOBE sırasında oluşacak otomatik şifreleme tetiklenmez ve bu da işletim sistemi varsayılanları yerine ilke tabanlı ayarların kullanılmasına izin verir




S Bir aygıt Intune ilkesinin uygulanması sonucunda şifrelenirse, bu ilke kaldırıldığında şifresi çözülür mü?

C: Şifreleme ile ilgili ilke kaldırılması, yapılandırılan sürücülerin şifresinin çözülmesiyle sonuçlanmaz.




S: Intune Uyumluluk ilkesi, aygıtımda "Bitlocker Etkin" olmadığını, ancak etkin olduğunu neden gösteriyor?

C: Intune uyumluluk ilkesinde "Bitlocker etkin" ayarı Windows Aygıt Durumu Attestation (DHA) istemcisini kullanır. Bu istemci yalnızca önyükleme zamanında aygıt durumunu ölçer. Bu nedenle, bitlocker şifrelemesi tamamlandığından beri bir aygıt yeniden başlatılmazsa, DHA istemci hizmeti bitlocker'ı etkin olarak bildirmez.