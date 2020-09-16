---
title: E-posta profillerini Intune ile kullanma
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
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653308"
---
# <a name="using-email-profiles-with-intune"></a>E-posta profillerini Intune ile kullanma

Intune, birden çok cihaz platformunda yerel (yerleşik) e-posta istemcisi için e-posta profilleri oluşturmak ve dağıtmak için kullanılabilir.

Var olan profillerin nasıl işlendiği ve e-posta profillerinin nasıl kaldırılacağı dahil olmak üzere e-posta profilleriyle ilişkilendirilmiş kısıtlamaların bazıları hakkında bilgi için, [Intune kullanarak aygıtlara e-posta ayarları ekleme](https://docs.microsoft.com/intune/email-settings-configure)konusuna bakın.

Her cihaz platformu için e-posta profili oluşturma hakkında daha fazla bilgi için bkz:

[Intune 'da e-postayı, kimlik doğrulamayı ve eşitlemeyi yapılandırmak için Android cihaz ayarları](https://docs.microsoft.com/intune/email-settings-android)  
[Microsoft Intune 'da iOS ve ıpados cihazları için e-posta ayarları ekleme](https://docs.microsoft.com/intune/email-settings-ios)  
[Windows Phone 8,1 çalıştıran cihazlarda Microsoft Intune 'da e-posta profili ayarları](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Microsoft Intune 'da Windows 10 çalıştıran cihazların e-posta profili ayarları](https://docs.microsoft.com/intune/email-settings-windows-10)

**Yaygın eşitleme sorunu**

**Android e-posta profilinde bir KNOX Kullanıcı kişilerinin, takvimin ve görevlerinin Kullanıcı aygıtlarına eşitlenmesini engeller.**

Android KNOX e-posta profilinde KNOX her biri etkin olarak ayarlanarak hangi içerik türlerinin cihaza eşitleneceğini belirleme seçeneğini belirtin.

İçerik türlerinden herhangi birinin ayarı **yapılandırılmazsa** (varsayılan olarak), bu içerik türü otomatik olarak eşitlenmez. Bir kullanıcı doğrudan cihazda doğrudan cihazda istedikleri içerik türünü etkinleştirebilir, ancak bu yapılandırmanın Intune ilke ayarı tarafından üzerine yazılır ve eşitleme bu içerik türü için durdurulur.

