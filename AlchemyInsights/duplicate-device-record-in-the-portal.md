---
title: Portalda yinelenen cihaz kaydı
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
- "9001495"
- "4386"
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004174"
---
# <a name="duplicate-device-record-in-the-portal"></a>Portalda yinelenen cihaz kaydı

Bir cihaz, ortak yönetimi durumunu Configuration Manager sitesine doğru şekilde bildirmezse, portalda bir cihaza ait 2 kayıt görebilirsiniz. Cihazın ortak yönetim durumunu denetlemek için Configuration Manager konsolunda cihazın **Ortak yönetilen** sütununu gözden geçirin. Sütun görünmüyorsa sütun başlıklarından herhangi birini sağ tıklayıp sütunu listeden seçerek ekleyebilirsiniz.

Ortak yönetilen değeri **Evet** olmalıdır. Değer **Hayır** ise istemci aygıtında Configuration Manager istemci uygulamasını açıp Genel sekmesindeki **Ortak yönetim** özelliğine bakın.

- Değer **Etkin** ise bu, Yönetim Noktasıyla istemci iletişiminde sorun olduğunu gösterir. Lütfen olası bağlantı sorunlarını araştırmak için cihazdaki **CcmMessaging.log** günlüğünü inceleyin.

- Değer **Devre dışı** ise ve cihaz Intune’a kayıtlıysa, lütfen cihazdaki **CoManagementHandler.log** günlüğünü gözden geçirerek cihazın Ortak yönetim ilkesini aldığından emin olun.
