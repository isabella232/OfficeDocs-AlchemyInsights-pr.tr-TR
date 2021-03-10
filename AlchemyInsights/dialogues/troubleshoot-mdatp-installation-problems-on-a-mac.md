---
title: Mac'te MDATP yükleme sorunlarını giderme
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696099"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Mac'te MDATP yükleme sorunlarını giderme

El ile yükleme başarısız **olursa, yükleme** sihirbazının Özet sayfası aşağıdaki hatayı gösterir:

"Yükleme sırasında bir hata oluştu. Yükleyici, yüklemenin başarısız olmasına neden olan bir hatayla karşılaştı. Yardım için yazılım üreticisine başvurun."

MDM dağıtımları için, sayfada genel yükleme hatası da görüntülenir.

Son kullanıcılara tam hatalar görüntülense de, **/Library/Logs/Microsoft/mdatp/install.log** dosyasında yükleme ilerlemesi olan bir günlük dosyası tutabilirsiniz. Her yükleme oturumu bu günlük dosyasının sonuna eklenir. Yalnızca son yükleme oturumunun çıkışını yapmak için `sed` kullanın.

Daha fazla bilgi edinmek için [Mac için Microsoft Defender ATP'de yükleme sorunlarını giderme makalesine bakın.](https://go.microsoft.com/fwlink/?linkid=2144615)
