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
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695378"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Ağ iletisi kimliğini sağlayarak e-posta iletisi gönderme

1. Yeni gönderim **uç bilgisinde,** E-posta **ve Ağ** **İletiSi Kimliği'ne seçin.**
2. Outlook'ta e-posta iletisi için ileti kimliğini bulmak için şu adımları izleyin:
    1. E-posta iletisine çift tıklayın ve açın.
    1. Dosya **Özellikleri'ne**  >  **tıklayın.**
    1. Not Defteri'ni veya boş bir Word belgesini açın ve görünürlüğü artırmak için **İnternet** üst bilgileri kutusunda bulunan içeriği kopyalayıp açık belgeye yapıştırın.
    1. **X-MS-Exchange-Organization-Network-Message-Id alanını** bulun. Bundan sonra gelen **değer:** gönderiniz için gereken kimliktir.
3. Alıcılar **altında,** e-posta bu e-postanın tüm alıcıları için gereksiz posta klasörüne inerse, **Seç'i seçin.** Yoksa, yalnızca sorunu bildiren kullanıcıyı seçin.
4. Gönderme **nedeni altında,** Engellenmiş olmalı seçeneğini belirtir, iletinin İstenmeyen  **Posta,** Kimlik Avı veya Kötü Amaçlı Yazılım olarak engellenmiş olup olmadığını belirtin ve gönder'i **seçin.** 

Daha fazla bilgi edinmek için [bkz. Tarama için şüpheli istenmeyen posta, kimlik avı, URL'ler ve dosyaları Microsoft'a gönderme.](https://go.microsoft.com/fwlink/?linkid=2101479)
