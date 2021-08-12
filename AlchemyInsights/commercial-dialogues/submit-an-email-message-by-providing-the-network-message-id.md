---
title: Ağ iletisi kimliğini sağlayarak e-posta iletisi gönderme
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1a6f9815a36cc267a815ff9757d713afed5d95aec4f7c537135c88cadf26cc51
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929937"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Ağ iletisi kimliğini sağlayarak e-posta iletisi gönderme

1. Yeni gönderim **uç iletisinde** E-posta ve **Ağ** İleti **Kimliği'ne seçin.**
2. E-posta iletisinde ileti kimliğini bulmak için şu adımları Outlook:
    1. E-posta iletisine çift tıklayın ve açın.
    1. Dosya **Özellikleri'ne**  >  **tıklayın.**
    1. Daha Not Defteri bir Word belgesi veya boş bir Word belgesi açın ve daha görünürlüğü artırmak için **internet** başlıkları kutusunda bulunan içeriği kopyalayıp açık belgeye yapıştırın.
    1. **X-MS-Exchange-Organization-Network-Message-Id alanını** bulun. : değerinden **sonra gelen** değer, gönderiniz için ihtiyacınız olan kimliktir.
3. Alıcılar **altında,** e-posta bu e-postanın tüm alıcıları için gereksiz posta klasörüne inerse, Select **All öğesini seçin.** Yoksa, yalnızca sorunu bildiren kullanıcıyı seçin.
4. Gönderme **nedeni'nin altında** , Engellenmiş olmalı öğesini seçerek iletinin **İstenmeyen** Posta **,** Kimlik Avı veya Kötü Amaçlı Yazılım olarak engellenmiş olup olmadığını belirtin ve sonra da Gönder'i **seçin.** 

Daha fazla bilgi edinmek için [bkz. Şüpheli istenmeyen posta, kimlik avı, URL'ler](https://go.microsoft.com/fwlink/?linkid=2101479)ve dosyaları tarama için Microsoft'a gönderme.
