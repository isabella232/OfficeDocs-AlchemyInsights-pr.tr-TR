---
title: Uygulama algılanmadı hatasını azaltma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666998"
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
