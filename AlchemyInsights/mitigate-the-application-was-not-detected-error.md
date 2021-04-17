---
title: Uygulama algılanmadı hatasını azaltma
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836371"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>"Uygulama algılanmadı" hatasını azaltma

Intune tarafından bildirilen uygulama yükleme hatası “Yükleme başarıyla tamamlandıktan sonra uygulama algılanmadı” tüm önemli işletim sistemi platformlarında (Windows, iOS ve Android) oluşabilir.

Bu hatayı oluşturan en yaygın senaryolar şunlardır:

- İlk dağıtımdan sonra uygulama Intune’un dışında güncelleştirildi (üçüncü taraf bir uygulama mağazasından). Örneğin Google Chrome gibi bazı uygulamalar otomatik güncelleştirmeler yapabilir.
- İlk yüklemeden sonra kullanıcı uygulamayı kaldırdı.

Bu sorunu azaltmak için önce etkilenen cihazları gözden geçirip hatanın oluştuğu senaryoyu saptayın.

- Uygulama Intune’un dışında güncelleştirildiyse, uygulama dağıtımı uygulama sürümünü yoksayacak şekilde ayarlanabilir. Bunu yapmak için **Uygulama Yapılandırması > Uygulama Bilgileri**’nin altında **Uygulama sürümünü yoksay** seçeneğini **Evet** olarak ayarlayın.
- İstemciyi hedeflerken uygulamayı “gerekli” olarak dağıtmak ve en son sürümün dağıtıldığından emin olmak uygun olabilir.
- Alternatif olarak, işletim sistemi platformunda Apple Volume Purchase Program ile ilişkilendirilmiş **autoupdate** işlevselliğini kullanmak mümkündür. Bu, kullanıma sunulan yeni uygulama sürümlerine otomatik güncelleştirme yapılacak şekilde yapılandırılabilir.

Uygulama yükleme sorunlarını giderme hakkında daha fazla bilgi için bkz. [Uygulama yükleme sorunlarını giderme](https://docs.microsoft.com/intune/troubleshoot-app-install).
