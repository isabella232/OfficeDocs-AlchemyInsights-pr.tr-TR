---
title: Intune ile e-posta profillerini kullanma
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555758"
---
# <a name="using-email-profiles-with-intune"></a>Intune ile e-posta profillerini kullanma

Intune, birden çok aygıt platformunda yerel (yerleşik) e-posta istemcisi için e-posta profilleri oluşturmak ve dağıtmak için kullanılabilir.

Varolan profillerin varlığının nasıl işlendiği ve e-posta profillerinin nasıl kaldırılılabildiğini içeren bazı kısıtlamalar hakkında bilgi için [bkz.](https://docs.microsoft.com/intune/email-settings-configure)

Her cihaz platformu için e-posta profilleri nin nasıl oluşturulabildiğini hakkında daha fazla bilgi için bkz:

[Intune'da e-posta, kimlik doğrulama ve senkronizasyon yapılandırmak için Android cihaz ayarları](https://docs.microsoft.com/intune/email-settings-android)  
[Microsoft Intune'da iOS ve iPadOS aygıtları için e-posta ayarları ekleme](https://docs.microsoft.com/intune/email-settings-ios)  
[Windows Phone 8.1 çalıştıran aygıtlar için Microsoft Intune'daki e-posta profil ayarları](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Microsoft Intune'da Windows 10 çalıştıran aygıtlar için e-posta profil ayarları](https://docs.microsoft.com/intune/email-settings-windows-10)

**Ortak eşitleme sorunu**

**Android e-posta profilindeki bir KNOX, kullanıcı Kişileri, Takvim ve Görevler'in kullanıcı aygıtlarına senkronize olmasını engeller.**

Android KNOX e-posta profilindeki KNOX, yöneticiye, her biri etkin olarak ayarlayarak hangi içerik türlerinin cihazla senkronize edildiğine karar verme seçeneği sunar.

İçerik türlerinden herhangi birinin ayarı **yapılandırılmamış** (varsayılan) olarak ayarlanmışsa, bu içerik türü otomatik olarak eşitlenmez. Kullanıcı doğrudan aygıtta istediği içerik türünü el ile etkinleştirebilir, ancak bu yapılandırma Intune ilke ayarı tarafından üzerine yazılır ve bu içerik türü için eşitleme durur.

