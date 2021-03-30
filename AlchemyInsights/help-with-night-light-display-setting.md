---
title: Gece ışığı ekran ayarıyla ilgili yardım
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405184"
---
# <a name="help-with-the-night-light-display-setting"></a>Gece ışığı ekran ayarıyla ilgili yardım

Windows 10'da gece saati görüntüleme ayarları hakkında daha fazla bilgi edinmek için bkz. [Ekranınızı gece için ayarlama.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)

Ayarlar'da gece ışığı seçenekleri gri görüntüleniyorsa ekran sürücüne bakın: 

1. Görev çubuğunuzda arama kutusuna tıklayın ve **Cihaz** Yöneticisi yazın ve ardından arama sonuçlarında **Cihaz** Yöneticisi'ni seçin.
1. Görüntü **bağdaştırıcılarını genişletin.** 

Cihazınız DisplayLink sürücüsü veya Temel Ekran sürücüsü kullanıyorsa gece ışığı özelliği kullanılamaz.

Gece ışığı özelliği en son grafik teknolojisini kullanır, bu nedenle ekran sürücünizi güncelleştirmeniz gerekir:  

- Güvenlik Windows Update'in **Güncelleştirmeleri**  >  **Denetleme'ye**  >  **& Ayarlar**  >  **Güncelleştirmesi'ne**  >  **gidip güncelleştirmeleri denetleme.**  

VEYA

- En son görüntü sürücülerini el ile indirmek ve yüklemek için donanım üreticinizin destek web sitesini ziyaret edin.

## <a name="reset-night-light-in-the-registry"></a>Kayıt defterinde gece ışığını sıfırlama

Ekran sürücü güncelleştirmeyi çalışmıyorsa kayıt defterinde gece ışığını sıfırlamanız gerekiyor olabilir.  

**Dikkat:** Bu sorun giderme adımı yalnızca ileri düzey kullanıcılar için önerilir. Kayıt defterinde yanlış bir değişiklik olursa, ciddi sorunlar oluşabilir. Ek koruma için, değişiklik yapmadan önce kayıt defterini yedeklenin, böylece sorun oluşursa geri yükleyebilirsiniz.

1. Arama kutusuna **regedit yazın ve ardından** arama sonuçlarında **Kayıt Defteri Düzenleyicisi'ni** seçin.

1. Aşağıdaki kayıt defteri anahtarına gidin: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Aşağıdaki alt anahtarı dışarı aktarın ve ardından silin:$$windows.data.bluelightreduction.bluelightreductionstate

1. Şu alt anahtarı dışarı aktarın ve ardından silin:$$windows.data.bluelightreduction.settings

1. Windows'u yeniden başlatın ve gece ışığı seçeneklerinin kullanılabilir olup olduğunu doğrulayın.


