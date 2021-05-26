---
title: Uç nokta DLP’sini yapılandırma
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657949"
---
# <a name="configure-endpoint-dlp"></a>Uç nokta DLP’sini yapılandırma

Microsoft Uç nokta DLP’si, Windows 10 cihazlarında DLP koruma ve izleme özelliğini hassas bilgilere kadar genişletmenize olanak sağlar. Cihazlar cihaz yönetimine eklendikten sonra, öğeler üzerinde koruyucu eylemler uygulamak amacıyla DLP ilkeleri oluşturabilirsiniz. Hassas öğelerle ilgili etkinlikleri izlemek için Etkinlik Gezgini kullanılabilir. Daha fazla bilgi için bkz. [Cihazları cihaz yönetimine ekleme](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Uç nokta DLP’sini kullanmaya başlamak için:

- Uygun SKU/abonelik lisansına sahip olduğunuzdan emin olun. Daha fazla bilgi için bkz. [SKU/abonelik lisansı](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Cihaz yönetimini etkinleştirmek, katılım sayfasına erişmek veya cihaz izlemeyi etkinleştirmek/devre dışı bırakmak için gerekli izinleri kontrol edin. Daha fazla bilgi için bkz. [İzinler](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Aşağıdaki cihaz ekleme yordamını izleyerek cihazları Cihaz yönetimine ekleyin. Daha fazla bilgi için bkz. [Cihazları ekleme](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Hassas öğelerinizi korumak için DLP ilkeleri oluşturun. Bilgi için bkz. [Uç nokta DLP ilkesi senaryoları](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Microsoft Uç nokta DLP’si hakkında daha fazla bilgi için bkz. [Microsoft 365 uç noktada veri kaybını önleme (önizleme) özelliği hakkında bilgi edinin](/microsoft-365/compliance/endpoint-dlp-learn-about).

**Destek gerekirse, Önemli Veri Toplama adımları:**

1. İstemci [Çözümleyicisi MDATP Önizlemesi'ne indirin.](https://aka.ms/betamdatpanalyzer)
1. Aracı cmd penceresinden Yönetici olarak çalıştırın:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. İzlemeleri toplamak **için dakika sayısını girin:** ile sorulsa, senaryoyu çalıştırmak için gereken dakika sayısını girin.
1. Senaryoyu çalıştırın.

Destek temsilcisine vermek için Zip dosyası çıkışını toplayın.
