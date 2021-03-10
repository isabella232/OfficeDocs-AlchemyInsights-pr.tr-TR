---
title: Uygulama uyumluluğu testi yapma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9138"
- "9005291"
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694861"
---
# <a name="do-app-compatibility-testing"></a>Uygulama uyumluluğu testi yapma

Microsoft Edge için uygulama uyumluluğu son derece yüksektir. Aslında, Microsoft'un aşağıdaki uyumluluk sözlerine sahip olması o kadar yüksektir:
- Microsoft Edge 45 ve önceki sürümlerde çalışıyorsa, Microsoft Edge 77 ve sonraki sürümlerde çalışır.
- Internet Explorer'da çalışıyorsa, Internet Explorer modunda Microsoft Edge'de çalışır.
- Google Chrome'da çalışıyorsa Microsoft Edge'de çalışır.

Bu söze uymayacak bir uygulamanız varsa, Microsoft App Assure ile bunu düzeltme sözünün [arkasındayız.](https://www.microsoft.com/fasttrack/microsoft-365/app-assure)

Bu söze rağmen, birçok kuruluşun bazı uygulamaları uyumluluk veya risk yönetimi nedenleriyle doğrulamaları gerektiğini biliyoruz. Bunun çok açık olmasını beklese de, uygulama testlerinden düzenli ve sıkı bir şekilde organize olmak önemlidir.

Uygulama uyumluluk testinin iki yolu vardır:

- **Laboratuvar testi:** Uygulamalar, belirli yapılandırmalarla sıkı denetimli bir ortamda test edilir.
- **Pilot test:** Uygulamalar, kendi cihazlarını kullanarak günlük çalışma ortamında sınırlı sayıda kullanıcı tarafından test edilir.

Her uygulama için en uygun yöntemi seçin ve tüm kuruluşa başlatmadan önce testi kullanın.

Uygulamalarınızı uyumlu olduğundan emin olduktan sonra, Microsoft Edge'i bir pilot gruba dağıtmaya hazır oluruz.
