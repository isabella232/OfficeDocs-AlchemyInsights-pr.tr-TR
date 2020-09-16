---
title: SharePoint Online terim deposunda terimler eksik
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
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750471"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Intune ile BitLocker şifrelemesini etkinleştirme

Intune, Intune kullanarak cihazları korumada açıklandığı gibi Windows cihazları için Boitkilitsiz şifreleme ayarlarını yapılandırmak için kullanılabilir.

Windows 10 çalıştıran yeni aygıtların, MDM ilkesinin uygulaması olmadan tetiklenen otomatik BitLocker şifrelemesini desteklemediğini bilmelisiniz. Bu, varsayılan ayarlar yapılandırılmadığında ilkenin uygulamasını etkileyebilir. Daha ayrıntılı bilgi için SSS bölümüne bakın.


SSS   : Windows 'un hangi sürümleri Endpoint Protection ilkesini kullanarak cihaz şifrelemeyi destekliyor mu?
 A: Intune Endpoint Protection Ilkesindeki ayarlar BitLocker CSP kullanılarak uygulanır.Windows 'un tüm sürümleri ve derlemeleri BitLocker CSP 'yi desteklemez. 
      Şu anda Windows sürümlerinde: Kurumsal; Eğitim, mobil, mobil kurumsal ve profesyonel (derleme 1809 sürümleri) desteklenir.




S: bir cihaz zaten BitLocker ile şifrelenmiş şifreleme yönteminin varsayılan ayarları ve şifreleme gücü (XTS-AES-128) kullanılarak şifrelenmişse, farklı ayarlarla ilke uygulanarak yeni ayarlarla sürücünün yeniden şifrelenmesi otomatik olarak ayarlanır.

Y: Hayır. Yeni şifre ayarlarını uygulamak için önce sürücünün şifresinin çözülmesi gerekir.

Autopilot ile kaydolan cihazların, Intune ilkesi değerlendirilinceye kadar otomatik şifreleme tetiklenemez ve bu da işletim sisteminin Varsayılanları yerine ilke tabanlı ayarların kullanılmasına izin verir




S Intune ilkesi uygulaması nedeniyle bir cihaz şifrelenmişse, bu ilke kaldırıldığında şifresi çözülür mi?

A: şifrelemeyle ilgili ilkenin kaldırılması, yapılandırılmış sürücülerin şifresinin çözülmesini sağlamaz.




S: Intune uyumluluk ilkesinde neden cihazımın "BitLocker etkin" olduğunu gösteriyor, ancak şu mu?

A: Intune uyumluluk ilkesindeki "BitLocker etkin" ayarı, Windows cihaz durumu kanıtlama (DHA) istemcisinin kullanır. Bu istemci yalnızca önyükleme sırasında cihaz durumunu ölçtüğünden. Bu nedenle, BitLocker şifrelemesi tamamlandığından bir cihaz yeniden başlatılıncaya kadar, DHA istemci hizmeti BitLocker 'ı etkin olduğu gibi bildirmeyecektir.