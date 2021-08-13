---
title: Liste öğeleriyle ilgili açıklamalar
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
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995527"
---
# <a name="comments-on-list-items"></a>Liste öğeleriyle ilgili açıklamalar

Kullanıcılar bir liste öğesiyle ilgili tüm yorumları süzer ve bir öğeyle ilgili açıklamalar veya etkinliğin görüntü olduğu görünümler arasında filtre uygulama.

Kullanıcıların açıklama ekp silebilirlerken önce şunları not etmek zorundaları gerekir:

- Açıklamalar, her ikisinde de izin ayarlarını SharePoint.
- Görev listeleri gibi modern kullanıcı arabirimlerinde henüz kurulmamış klasik listeler, bu açıklama özelliğine sahip olmaz.
- E-Teams listelerine açıklama ek olarak bu sürümde kullanılamaz.
- Açıklamalar Arama tarafından dizine almaz.

Yöneticiler **Set-SPOTenant** PowerShell cmdlet'inde **CommentsOnListItemsDisabled** parametresini değiştirerek kuruluş düzeyinde bu özelliği devre dışı bırakabilir.

Şu anda site veya liste düzeyinde açıklamayı devre dışı bırakmak mümkün değildir. Bu denetimlerin daha sonraki bir güncelleştirmede, büyük olasılıkla 2021'in ilk çeyreğinde sahip olmalarını umuyoruz.
