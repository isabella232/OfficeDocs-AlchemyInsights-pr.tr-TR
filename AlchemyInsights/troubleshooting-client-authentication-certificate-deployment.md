---
title: Sorun giderme İstemci Kimlik Doğrulama sertifika dağıtımı
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555806"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Sorun giderme İstemci Kimlik Doğrulama sertifika dağıtımı

Intune NDES/SCEP ve PKCS/PFX Client sertifikaları profilleri, kullanıcıların şirket kaynaklarına kimlik doğrulamasına olanak sağlamak için Wifi, VPN ve e-posta gibi diğer profil türleri ile birlikte yaygın olarak kullanılır. Bu profil türleri bir istemci sertifikası profiline bağlandığında, bu profilin başarılı bir şekilde dağıtılmasına bağlıdır.

İlk altyapı kurulumu ve İstemci Sertifikası profilinin ilişkili yapılandırması genellikle sorun giderme gerektirir. SERTIFIKA dağıtımıyla ilgili sorunları yalıtmak için NDES bağlayıcısının başarılı bir şekilde kurulumu ve sorun giderme kılavuzu için adım adım kılavuz için bkz: 

- [Intune ile SCEP'i destekleyecek altyapıyı yapılandırın](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Microsoft Intune ile Sorun Giderme SCEP sertifika profillerine genel bakış](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Yapılandırmanızı doğrulamaya yardımcı olmak için başvurulan powershell komut dosyalarını kullanın. Daha fazla bilgi için [Intune Certificate bağlayıcı sıyrık doğrulama komut dosyalarına](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)bakın.

  
**Diğer yaygın sorunlar**

**NDES bağlayıcı sunucusuna Intune sertifika bağlayıcısını yüklemeye çalıştığımda, "Sertifika isteğindeki parola doğrulanamıyor. Zaten kullanılmış olabilir. Bu istekle göndermek için yeni bir parola edinin."**  

Bu ileti, sertifika bağlayıcısı yüklemesini Yönetici olarak çalıştırmanız gerektiği anlamına gelir.

Bazı ortamlarda, Intune Sertifikası'nın çalıştığı sunucuların Intune'a bağlanmak için bir proxy sunucusu kullanması ve bu nedenle Sertifika Bağlayıcısı'nın bir proxy kullanması gerekir. Bazı durumlarda, NDES Bağlayıcısı yapılandırılan proxy ayarlarını yoksayarlar ve LocalSystem'in güvenlik bağlamında çalışırken proxy ayarlarını yapılandırmak gerekebilir. 
 
Çözüm System olarak Internet Explorer çalıştırmak ve IE bir proxy yapılandırmaktır. Intune Bağlayıcı Hizmetiyeniden başladıktan sonra NDES Bağlayıcısı Intune'a bağlanır.

**Kullanıcı aygıtları artık NDES'ten SCEP sertifikaları almıyor.**

NDES sunucusuna verilen ve NDES bağlayıcıyüklemesi sırasında belirtilen İstemci Kimlik Doğrulama sertifikasının süresi dolmuş veya eksik olabilir. Çözmek için: 
 
1. NDES konektörünü kaldırın.  
2. Yeni bir istemci kimlik doğrulama veya sunucu kimlik doğrulama sertifikası istemek için bu ayrıntıları kullanın: 
 
    - Konu adı: CN=external fqdn  
    - Özne alternatif adı (her ikisi de gereklidir): DNS=dış fqdn, DNS=iç fqdn 
 
3. NDES konektörünü yeni sertifikayla yeniden yükleyin.