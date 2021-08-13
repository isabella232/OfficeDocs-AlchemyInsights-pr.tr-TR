---
title: Intune ile e-posta profillerini kullanma
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
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919443"
---
# <a name="using-email-profiles-with-intune"></a>Intune ile e-posta profillerini kullanma

Intune, birden çok cihaz platformunda yerel (yerleşik) e-posta istemcisi için e-posta profilleri oluşturmak ve dağıtmak için kullanılabilir.

Mevcut profillerin iletişim durumu ve e-posta profillerinin nasıl kaldırılası dahil olmak üzere e-posta profilleriyle ilişkili kısıtlamaların bazıları hakkında bilgi için bkz. [Intune](https://docs.microsoft.com/intune/email-settings-configure)kullanarak cihazlara e-posta ayarları ekleme.

Her cihaz platformu için e-posta profilleri oluşturma hakkında daha fazla bilgi için bkz:

[Intune'da e-postayı, kimlik doğrulamayı ve eşitlemeyi yapılandırmak için Android cihaz ayarları](https://docs.microsoft.com/intune/email-settings-android)  
[Microsoft Intune'te iOS ve iPadOS cihazları için e-posta ayarları ekleme](https://docs.microsoft.com/intune/email-settings-ios)  
[Microsoft Intune 8.1 çalıştıran cihazlar için Windows Phone-posta profili ayarları](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[E-posta ile çalışan cihazlar için Windows 10 profil Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Yaygın eşitleme sorunu**

**Android e-posta profilinde KNOX, kullanıcının Kişiler, Takvim ve Görevler'in kullanıcı cihazlarıyla eşitlenesini önler.**

Android KNOX e-posta profilinde KNOX, yöneticiye hangi içerik türlerinin cihazla eşitli olduğuna karar verme seçeneği sunar. Bunun için her biri etkin olmalıdır.

İçerik türlerinden herhangi biri için ayar  Yapılandırılmadı (varsayılan) olarak ayarlanırsa, bu içerik türü otomatik olarak eşitlanmaz. Kullanıcı, doğrudan cihaz üzerinde kullanmak istediğiniz içerik türünü el ile etkinleştirebilir, ancak Intune ilke ayarı bu yapılandırmanın üzerine yazılır ve bu içerik türü için eşitleme durur.

