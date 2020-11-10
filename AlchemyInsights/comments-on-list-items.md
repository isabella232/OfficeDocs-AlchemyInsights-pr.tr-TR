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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982554"
---
# <a name="comments-on-list-items"></a>Liste öğeleri hakkında açıklamalar

Kullanıcılar yakında liste öğelerine açıklama ekleyebilir ve bunları silebilir. Kullanıcılar liste öğesindeki tüm açıklamaları görüntüleyebilir ve öğeyle ilgili açıklamaları veya etkinlikleri gösteren görünümler arasında filtre uygulayabilir.

**Zamanlama** :

**Hedeflenen sürüm** : orta Ekim 'de dereceli olarak alınan ve PARÇAAL-Kasım tarafından tamamlanması beklenen

**Standart sürüm** : PARÇAAL-Kasım ' da aşamalı toplama ve ilk Aralık ile tamamlanması bekleniyor

Kuruluş **: kuruluşun** tamamı için hedeflenen sürüm

Kullanıcıların açıklamaları ekleyip silebilmeleri için aşağıdakileri not etmeleri gerekir:

- Açıklamalar SharePoint 'te devralınan izin ayarlarını izler.
- Görev listeleri gibi modern kullanıcı arabirimlerinde gösterilecek henüz oluşturulmamış klasik listeler bu yorum özelliğini içermez.
- Ekipte bulunan listelere açıklama eklemek bu sürümde kullanılamaz.
- Açıklamalar, arama tarafından dizine alınır.

Yöneticiler, **set-SPOTenant** PowerShell cmdlet 'inde **CommentsOnListItemsDisabled** parametresini değiştirerek bu özelliği kuruluş düzeyinde devre dışı bırakabilir.

Site veya liste düzeyinde açıklama oluşturmayı devre dışı bırakmak mümkün değildir. Bu denetimlerin, büyük olasılıkla ilk çeyrek 2021 bu denetimlerden bir sonraki güncelleştirmede da yer almak isteriz.
