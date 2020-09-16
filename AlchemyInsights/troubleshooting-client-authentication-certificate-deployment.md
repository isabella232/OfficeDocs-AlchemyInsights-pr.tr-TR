---
title: Istemci kimlik doğrulama sertifikası dağıtımında sorun giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659006"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Istemci kimlik doğrulama sertifikası dağıtımında sorun giderme

Intune NDES/SCEP ve PKCS/PFX Istemci sertifikaları profilleri, kullanıcıların şirket kaynaklarını doğrulamasına olanak tanımak için WiFi, VPN ve e-posta gibi diğer profil türleriyle birlikte yaygın olarak kullanılır. Bu profil türleri bir istemci sertifikası profiliyle bağlantılıysa, bu profilin başarılı dağıtımına bağlıdır.

Istemci sertifikası profilinin ilk altyapı kurulumu ve ilişkili yapılandırması genellikle sorun giderme gerektirir. Bir adım adım kılavuz için, NDES Bağlayıcısı ve sorun giderme kılavuzunun sertifika dağıtımıyla ilgili sorunları yalıtmak için, bkz: 

- [Intune ile SCEP desteği için altyapıyı yapılandırma](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Microsoft Intune ile SCEP sertifika profillerinde sorun gidermeye genel bakış](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Yapılandırmanızı doğrulamaya yardımcı olması için başvurulan PowerShell betiklerini kullanın. Daha fazla bilgi için bkz: [Intune sertifika Bağlayıcısı doğrulama komut dosyaları](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Diğer yaygın sorunlar**

**NDES Connector sunucusuna Intune sertifika bağlayıcısını yüklemeye çalıştığımda, "sertifika isteğindeki parola doğrulanamıyor" iletisi alıyorum. Zaten kullanılmış olabilir. Bu istekle göndermek için yeni bir parola alın. "**  

Bu ileti, sertifika Bağlayıcısı yüklemesini yönetici olarak çalıştırmanız gerektiği anlamına gelir.

Bazı ortamlarda Intune sertifikasının çalıştığı sunucular Intune 'a bağlanmak için bir ara sunucu kullanmalıdır ve böylece sertifika bağlayıcısının bir proxy kullanması gerekir. Bazı durumlarda, NDES Bağlayıcısı yapılandırılmış proxy ayarlarını yoksayar ve LocalSystem güvenlik bağlamında çalışırken proxy ayarlarını yapılandırmak gerekebilir. 
 
Çözüm, Internet Explorer 'ı SISTEM olarak çalıştırmak ve IE 'de bir proxy yapılandırmaktır. Intune bağlayıcı hizmeti yeniden başlatıldıktan sonra, NDES Bağlayıcısı Intune 'a bağlanır.

**Kullanıcı cihazları artık NDES 'den SCEP sertifikası almıyor.**

NDES sunucusuna verilen ve NDES Bağlayıcısı yüklemesi sırasında belirtilen Istemci kimlik doğrulama sertifikasının süresi dolmuş veya yok olabilir. Çözmek için: 
 
1. NDES bağlayıcısını kaldırın.  
2. Yeni bir istemci kimlik doğrulaması veya sunucu kimlik doğrulama sertifikası istemek için bu ayrıntıları kullanın: 
 
    - Konu adı: CN = dış FQDN  
    - Konu alternatif adı (ikisi de gereklidir): DNS = dış FQDN, DNS = iç FQDN 
 
3. NDES bağlayıcısını yeni sertifikayla yeniden yükleyin.