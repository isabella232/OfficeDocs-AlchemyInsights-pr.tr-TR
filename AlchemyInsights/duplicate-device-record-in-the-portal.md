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
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814536"
---
# <a name="duplicate-device-record-in-the-portal"></a>Portalda yinelenen cihaz kaydı

Bir cihaz, ortak yönetimi durumunu Configuration Manager sitesine doğru şekilde bildirmezse, portalda bir cihaza ait 2 kayıt görebilirsiniz. Cihazın ortak yönetim durumunu denetlemek için Configuration Manager konsolunda cihazın **Ortak yönetilen** sütununu gözden geçirin. Sütun görünmüyorsa sütun başlıklarından herhangi birini sağ tıklayıp sütunu listeden seçerek ekleyebilirsiniz.

Ortak yönetilen değeri **Evet** olmalıdır. Değer **Hayır** ise istemci aygıtında Configuration Manager istemci uygulamasını açıp Genel sekmesindeki **Ortak yönetim** özelliğine bakın.

- Değer **Etkin** ise bu, Yönetim Noktasıyla istemci iletişiminde sorun olduğunu gösterir. Lütfen olası bağlantı sorunlarını araştırmak için cihazdaki **CcmMessaging.log** günlüğünü inceleyin.

- Değer **Devre dışı** ise ve cihaz Intune’a kayıtlıysa, lütfen cihazdaki **CoManagementHandler.log** günlüğünü gözden geçirerek cihazın Ortak yönetim ilkesini aldığından emin olun.
