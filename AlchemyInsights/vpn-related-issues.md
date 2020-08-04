---
title: VPN ile ilgili sorunlar
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555742"
---
# <a name="vpn-related-issues"></a>VPN ile ilgili sorunlar

MDM istemcileri için VPN bağlantısının başarılı bir şekilde uygulanması, VPN altyapısının gereksinimlerini doğru şekilde yansıtan dağıtılmış bir profile bağlıdır. Araştırdığınız istemci platformları için uygun ayarlar için bkz: 

[Intune kullanarak VPN bağlantıları eklemek için Windows 10 ve Windows Holografik cihaz ayarları](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Microsoft Intune'da iOS ve iPadOS aygıtlarında VPN ayarları ekleme](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Intune VPN yapılandırmak için Android cihaz ayarları](https://docs.microsoft.com/intune/vpn-settings-android)  
[Microsoft Intune'daki macOS aygıtlarında VPN ayarları ekleme](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

VPN profiliniz sertifika tabanlı kimlik doğrulaması kullanıyorsa, VPN profiline bağlı kök sertifika ve istemci kimlik doğrulama sertifikası profillerinin başarıyla dağıtıldıklarından emin olun.

**Sık Karşılaşılan Sorunlar**

**Bir cihaza VPN profili dağıttım. Intune başarılı olduğunu gösteriyor, ancak cihaz VPN'e bağlanmıyor.**

Başarılı bir durum, Intune'un profili yapılandırılmış olarak başarıyla dağıtmış olduğu anlamına gelir. Ancak, bu yapılandırmalar ağınız ve/veya kimlik doğrulama gereksinimleriniz ile eşleşmeyebilir. Altyapı ve kimlik doğrulama hizmetindeki günlükleri (VPN sunucusunda ve NPS/Radius sunucusunda) inceleyin ve bağlantı girişimi hakkında daha fazla bilgi sağlayın. Günlükleri toplamak ve incelemek için ağ altyapı ekibiniz veya üçüncü taraf VPN satıcınızla çalışmanız gerekebilir.

**iOS için özel bir VPN yapılandırdığımda, uygulama başına VPN özelliği kullanıma sunulmadı.**

Intune'daki iOS aygıtları için uygulama başına VPN şu anda, uygulama başına VPN'i yapılandırmadan önce sertifika ön koşullarını karşılaması gereken belirli bir sağlayıcı lar ve iş ortakları listesi için kullanılabilir. Daha fazla bilgi için bkz: [Intune'daki iOS/iPadOS aygıtları için uygulama başına Sanal Özel Ağ (VPN) ayarlayın.](https://docs.microsoft.com/intune/vpn-setting-configure-per-app) 

Intune'daki tüm VPN bağlantı türleri hakkında daha fazla bilgi için, [Intune'daki VPN sunucularına bağlanmak için VPN profilleri oluştur'a](https://docs.microsoft.com/intune/vpn-settings-configure)bakın.  

**iOS İsteğe Bağlı VPN, yapılandırılmış bir etki alanına erişildiğinde tetiklenmiyor**

Otomatik VPN ayarlarını test etmek için aşağıdaki değerleri ayarlayın:

Aşağıdakileri yapmak istiyorum: **Her bağlantı girişimini değerlendirin** 

Bağlanıp bağlanmayın: **Gerekirse bağlanın**

Kullanıcılar bu etki alanına erişirken: **hedef** *alan adı*

Yukarıdaki yapılandırma başarılı değilse, aşağıdaki öğeyi ekleyin:

Bu URL'ye erişimediğinde, VPN'i bağlamakuvvetine ulaşın: **BADURL**