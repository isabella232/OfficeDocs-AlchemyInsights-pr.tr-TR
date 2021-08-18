---
title: Intune’dan verileri kaldırma ve cihazları silme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: 92673c4a2a0e0faa98d3ade5ca1f6aa687d4c94a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331061"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Intune’dan verileri kaldırma ve cihazları silme

Cihaz Devre Dışı Bırakma ve Cihaz Silme uzak eylemleri Inture tarafından yönetilen şirket verilerini kaldırmak veya bir fabrika sıfırlaması yapıp cihazı varsayılan ayarlarına döndürmek için kullanılabilir.

1. Microsoft 365 Cihaz Yönetimi’nde oturum açın ve **Cihazlar** > **Tüm Cihazlar**’a gidin.
2. Silmek istediğiniz cihazı seçin.
3. Yapmak istediğiniz uzaktan silme türünü seçin. Devre dışı bırakma işlemi yalnızca kurumsal bilgileri silerken, tam silme işlemi cihazı fabrika ayarlarına geri yükler.
4. Onaylamak için **Evet**'i seçin. Silme işlemi bitene kadar Cihazın eylem durumu *Devre Dışı Bırakma Bekliyor* olarak gösterilir.
    Eylem tamamlandıktan sonra artık yönetilen cihaz listesinde mobil cihazı görmezsiniz.

**Not:** Şirket verileri Azure AD'ye KATıLMıŞ cihazlardan kaldırılamaz. 

Devre Dışı Bırakma ve Silme eylemlerinin etkisiyle ilgili olarak, nelerin tutulduğu ve nelerin silindiği de dahil olmak üzere tüm ayrıntılar için aşağıdaki belgelere bakın:

- [Silme veya devre dışı bırakma işlemlerini kullanarak ya da cihazın kaydını el ile kaldırarak cihazları kaldırma](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Intune tarafından yönetilen uygulamalardan yalnızca kurumsal verileri silme](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [macOS cihazından tüm verileri silme](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).