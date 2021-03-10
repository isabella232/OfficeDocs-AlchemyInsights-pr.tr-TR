---
title: Kiracı ilkesi düzeltme (eylem geçersiz kılma)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695690"
---
# <a name="fix-tenant-policy-action-override"></a>Kiracı ilkesi düzeltme (eylem geçersiz kılma)

Kiracınıza gelen istenmeyen posta önleme ilkesi bu iletiyi etkiledi. İlkeyi gözden geçirmek için şunları yapın:

1. [Office 365 Güvenlik ve Uyumluluk &'ne](https://go.microsoft.com/fwlink/p/?linkid=2077143)gidin ve ardından Tehdit yönetimi İlkesi İstenmeyen Postayla   >    >  [Mücadele'ye gidin.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. İlke kaynağının **şunları gösterir** olup olmadığını kontrol edin:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC iletisi**

    Öyleyse, Özel **sekmesinde** iletiyi etkilenen ilkenin ayarlarını kontrol edin. Tüm Exchange Online Protection **müşterilerine uygulanan** Standart ayarlar iletiyi etkilemektedir.

İstenmeyen posta filtresi ilkelerini yapılandırma hakkında daha fazla bilgi için bkz. [İstenmeyen posta filtresi ilkelerinizi yapılandırma.](https://go.microsoft.com/fwlink/?linkid=2101431)
