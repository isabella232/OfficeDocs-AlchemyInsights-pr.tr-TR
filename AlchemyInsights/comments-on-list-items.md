---
title: Liste öğeleri hakkında açıklamalar
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724174"
---
# <a name="comments-on-list-items"></a>Liste öğeleri hakkında açıklamalar

Kullanıcılar liste öğesindeki tüm açıklamaları görüntüleyebilir ve öğeyle ilgili açıklamaları veya etkinlikleri gösteren görünümler arasında filtre uygulayabilir.

Kullanıcıların açıklamaları ekleyip silebilmeleri için aşağıdakileri not etmeleri gerekir:

- Açıklamalar SharePoint 'te devralınan izin ayarlarını izler.
- Görev listeleri gibi modern kullanıcı arabirimlerinde gösterilecek henüz oluşturulmamış klasik listeler bu yorum özelliğini içermez.
- Ekipte bulunan listelere açıklama eklemek bu sürümde kullanılamaz.
- Açıklamalar, arama tarafından dizine alınır.

Yöneticiler, **set-SPOTenant** PowerShell cmdlet 'inde **CommentsOnListItemsDisabled** parametresini değiştirerek bu özelliği kuruluş düzeyinde devre dışı bırakabilir.

Site veya liste düzeyinde açıklama oluşturmayı devre dışı bırakmak mümkün değildir. Bu denetimlerin, büyük olasılıkla ilk çeyrek 2021 bu denetimlerden bir sonraki güncelleştirmede da yer almak isteriz.
