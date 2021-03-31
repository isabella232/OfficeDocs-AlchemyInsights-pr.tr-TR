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
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402463"
---
# <a name="configure-endpoint-dlp"></a>Uç nokta DLP’sini yapılandırma

Microsoft Uç nokta DLP’si, Windows 10 cihazlarında DLP koruma ve izleme özelliğini hassas bilgilere kadar genişletmenize olanak sağlar. Cihazlar cihaz yönetimine eklendikten sonra, öğeler üzerinde koruyucu eylemler uygulamak amacıyla DLP ilkeleri oluşturabilirsiniz. Hassas öğelerle ilgili etkinlikleri izlemek için Etkinlik Gezgini kullanılabilir. Daha fazla bilgi için bkz. [Cihazları cihaz yönetimine ekleme](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Uç nokta DLP’sini kullanmaya başlamak için:

- Uygun SKU/abonelik lisansına sahip olduğunuzdan emin olun. Daha fazla bilgi için bkz. [SKU/abonelik lisansı](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Cihaz yönetimini etkinleştirmek, katılım sayfasına erişmek veya cihaz izlemeyi etkinleştirmek/devre dışı bırakmak için gerekli izinleri kontrol edin. Daha fazla bilgi için bkz. [İzinler](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Aşağıdaki cihaz ekleme yordamını izleyerek cihazları Cihaz yönetimine ekleyin. M365 Uyumluluk **Ayarları** altında Cihaz Ekleme (önizleme) seçeneği bulunmuyorsa, yukarıda bahsedilen uygun lisansa ve izinlere sahip olduğunuzu onaylayın. Daha fazla bilgi için bkz. [Cihazları ekleme](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Hassas öğelerinizi korumak için DLP ilkeleri oluşturun. Bilgi için bkz. [Uç nokta DLP ilkesi senaryoları](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Microsoft Uç nokta DLP’si hakkında daha fazla bilgi için bkz. [Microsoft 365 uç noktada veri kaybını önleme (önizleme) özelliği hakkında bilgi edinin](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Destek gerekirse, Önemli Veri Toplama adımları:**

1. MDATP Client Analyzer Preview aracını [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer") adresinden indirin
2. Aracı cmd penceresinden Yönetici olarak çalıştırın:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. “İzlemeleri toplamak için gereken dakika sayısını girin:” istemi göründüğünde, senaryoyu çalıştırmak için gereken dakika sayısını girin
5. Senaryoyu çalıştırın

Destek temsilcisine verilecek Zip dosyası çıkışını toplayın.
