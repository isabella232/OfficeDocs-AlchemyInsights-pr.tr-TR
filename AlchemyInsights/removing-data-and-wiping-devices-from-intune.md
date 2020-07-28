---
title: Verileri kaldırma ve cihazları Intune'dan silme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440463"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Verileri kaldırma ve cihazları Intune'dan silme

Aygıt Emekli Ve Aygıt Silme uzak eylemleri, Intune tarafından yönetilen şirket verilerini kaldırmak veya fabrika sıfırlama gerçekleştirmek ve aygıtı varsayılan ayarlarına döndürmek için kullanılabilir.

1. Microsoft 365 Aygıt Yönetimi'nde oturum açın ve **Tüm Aygıtlar**  >  **Aygıtları'na**gidin.
2. Silmek istediğiniz aygıtı seçin.
3. Yapmak istediğiniz uzaktan silme türünü seçin. Retire yalnızca kuruluş bilgilerini silerken, tam silmeler aygıtı fabrika ayarlarına geri yüklenir.
4. Onaylamak için **Evet'i** seçin. Silme bitene kadar, Aygıt eylem durumu Bekleyen Emekli olarak gösterir.</br>
    Eylem tamamlandıktan sonra, mobil aygıtı artık yönetilen aygıt listesinde görmezsiniz.

**Not** Şirket verileri, Azure AD'ye katılan aygıtlardan kaldırılamaz.

Nelerin tutulduğu ve silindiği de dahil olmak üzere Emekli Ve Sil eylemlerinin [etkisinin](https://docs.microsoft.com/intune/devices-wipe)tüm ayrıntıları için bkz.

MacOS aygıtından tüm verileri silmek için [bkz.](https://docs.microsoft.com/intune/device-erase)