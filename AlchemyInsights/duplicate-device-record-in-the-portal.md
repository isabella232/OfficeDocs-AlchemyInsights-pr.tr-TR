---
title: Portalda yinelenen cihaz kaydı
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790177"
---
# <a name="duplicate-device-record-in-the-portal"></a>Portalda yinelenen cihaz kaydı

Bir cihaz, ortak yönetimi durumunu Configuration Manager sitesine doğru şekilde bildirmezse, portalda bir cihaza ait 2 kayıt görebilirsiniz. Cihazın ortak yönetim durumunu denetlemek için Configuration Manager konsolunda cihazın **Ortak yönetilen** sütununu gözden geçirin. Sütun görünmüyorsa sütun başlıklarından herhangi birini sağ tıklayıp sütunu listeden seçerek ekleyebilirsiniz.

Ortak yönetilen değeri **Evet** olmalıdır. Değer **Hayır** ise istemci aygıtında Configuration Manager istemci uygulamasını açıp Genel sekmesindeki **Ortak yönetim** özelliğine bakın.

- Değer **Etkin** ise bu, Yönetim Noktasıyla istemci iletişiminde sorun olduğunu gösterir. Lütfen olası bağlantı sorunlarını araştırmak için cihazdaki **CcmMessaging.log** günlüğünü inceleyin.

- Değer **Devre dışı** ise ve cihaz Intune’a kayıtlıysa, lütfen cihazdaki **CoManagementHandler.log** günlüğünü gözden geçirerek cihazın Ortak yönetim ilkesini aldığından emin olun.
