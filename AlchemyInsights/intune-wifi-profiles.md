---
title: Intune Wi-Fi profilleri
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555817"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi profilleri

MDM istemcileri için Wi-Fi bağlantısının başarılı bir şekilde uygulanması, kurumsal Wi-Fi altyapısının gereksinimlerini yansıtan doğru şekilde dağıtılan bir profile bağlıdır. Araştırdığınız istemci platformları için uygun ayarları gözden geçirmek için bkz: 

[Microsoft Intune'da Android çalıştıran cihazlar için Wi-Fi ayarları ekleme](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Microsoft Intune'da Android Enterprise'a özel ve tam olarak yönetilen cihazlar için Wi-Fi ayarları ekleme](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Microsoft Intune'da iOS ve iPadOS aygıtları için Wi-Fi ayarları ekleme](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Intune'da Windows 10 ve sonraki aygıtlar için Wi-Fi ayarları ekleme](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Intune'daki Windows aygıtları için Wi-Fi ayarlarını alma](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Sık Karşılaşılan Sorunlar**

**Wi-Fi profilinde belirtilen dağıtılmış sertifikaya bağlı bir Wi-Fi profili dağıtıyorum. Ancak, yapılandırma profilleri bir hata durumu gösteriyor.**

Cihazınızın sertifikayı aldığından kontrol edin.

1. Intune'da **Tüm Aygıtlar'a** gidin ve aygıt > **Aygıtı'nı**seçin.

2. Beklenen tüm profillerin listelenmiş ve başarılı bir durumda olup olmadığını denetleyin.

3. Android profili için, sertifika zincirinizde ara sertifikalar varsa, bunların Android cihazlara dağıtıldıklarından emin olun.

    Sertifika durumunu kontrol etmek için **Aygıt yapılandırma**  >  **Profilleri**Android ara  >  **CA**  >  **Özellikleri**  >  **Güvenilir Sertifika'ya**gidin.

Hataları görmeye devam ederseniz, yordamları ve sorun giderme bölümlerini gözden geçirin. Daha fazla bilgi için Microsoft [Intune ile sorun giderme SCEP sertifika profilleri için Genel Bakış'a](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)bakın.

**Bir cihaza Wi-Fi profili dağıttım. Intune başarılı olduğunu gösteriyor, ancak cihaz Wi-Fi'a bağlanmıyor.**

Başarılı bir durum, Intune'un profili yapılandırılmış olarak başarıyla dağıtmış olduğu anlamına gelir. Ancak, bu yapılandırmalar ağınız ve/veya kimlik doğrulama gereksinimleriniz ile eşleşmeyebilir. Bağlantı girişimi hakkında daha fazla bilgi için, altyapı ve kimlik doğrulama hizmetindeki (Wi-Fi Access noktası denetleyicisi ve NPS/Radius sunucusunda) günlükleri gözden geçirin. Günlükleri toplamak ve incelemek için ağ altyapı ekibinizle veya üçüncü taraf Wi-Fi satıcısıyla çalışmanız gerekebilir.