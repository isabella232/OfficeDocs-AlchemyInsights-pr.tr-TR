---
title: İstemci Kimlik Doğrulaması sertifika dağıtımı sorunlarını giderme
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
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020824"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>İstemci Kimlik Doğrulaması sertifika dağıtımı sorunlarını giderme

Intune NDES/SCEP ve PKCS/PFX Client sertifikaları profilleri, kullanıcıların şirket kaynaklarında kimlik doğrulaması yapmalarını sağlayan WiFi, VPN ve e-posta gibi diğer profil türleriyle birlikte yaygın olarak kullanılır. Bu profil türleri bir istemci sertifika profiline bağlı olduğunda, bu profilin başarıyla dağıtımına bağlıdır.

İstemci Sertifikası profilinin ilk altyapısının kurulumu ve ilişkili yapılandırması genellikle sorun giderme gerektirir. Sertifika dağıtımıyla ilgili sorunları yalıtmak için NDES bağlayıcısını ve sorun giderme kılavuzunu başarılı bir şekilde ayarlamaya yönelik adım adım kılavuz için bkz: 

- [Intune ile SCEP'yi desteklemek için altyapıyı yapılandırma](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [SCEP sertifika profillerini ve güvenlik sorunlarını gidermeye genel Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Yapılandırmanızı doğrulamaya yardımcı olmak için başvurulan PowerShell betiklerini kullanın. Daha fazla bilgi için [bkz. Intune Sertifika bağlayıcısı doğrulama betikleri.](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)

  
**Diğer yaygın sorunlar**

**Intune sertifika bağlayıcısını NDES bağlayıcısı sunucusuna yüklemeye çalışarak "Sertifika isteğinde parola doğrulanamıyor. Daha önce kullanılmış olabilir. Bu istekle göndermek için yeni bir parola alın".**  

Bu ileti, sertifika bağlayıcısı yüklemesini Yönetici olarak çalıştırmanız gereken anlamına gelir.

Bazı ortamlarda, Intune Sertifikası'nın çalıştır olduğu sunucuların Intune'a bağlanmak için bir ara sunucu kullanmaları ve dolayısıyla Sertifika Bağlayıcısı'nın bir proxy kullanması gerekir. Bazı durumlarda, NDES Bağlayıcısı yapılandırılmış ara sunucu ayarlarını yoksayar ve LocalSystem'ın güvenlik bağlamında çalışırken proxy ayarlarını yapılandırmanız gerekebilir. 
 
Çözüm, Internet Explorer'ı SYSTEM olarak çalıştırmak ve IE'de bir proxy yapılandırmaktır. Intune Bağlayıcı Hizmeti yeniden başlatıldıktan sonra, NDES Bağlayıcısı Intune'a bağlanır.

**Kullanıcı cihazları artık NDES'den SCEP sertifikası almıyor.**

NDES sunucusuna verilen ve NDES bağlayıcısı yüklemesi sırasında belirtilen İstemci Kimlik Doğrulaması sertifikasının süresi dolmuş veya eksik olabilir. Bu sorunu çözmek için: 
 
1. NDES bağlayıcıyı kaldırın.  
2. Yeni bir istemci kimlik doğrulaması veya sunucu kimlik doğrulaması sertifikası talep etmek için bu ayrıntıları kullanın: 
 
    - Konu adı: CN=dış fqdn  
    - Konu alternatif adı (her ikisi de gereklidir): DNS=dış fqdn, DNS=iç fqdn 
 
3. NDES bağlayıcısını yeni sertifikayla yeniden yükleyin.