---
title: Dolandırıcılık algılama denetimleri için güvenlik ipucu sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834751"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Dolandırıcılık algılama denetimleri için güvenlik ipucu sorunlarını giderme

"Gönderen, dolandırıcılık algılama denetimlerimizi başarısız yaptı" ifadesinin yer alma olduğu bir güvenlik ipucu alıyorsanız ve bu gönderen, DKIM veya SPF kimlik doğrulama denetimlerinden geçiremedi. Bunu çözmek için en iyi yöntem, gönderenin kendi yetkilerini vermesidir. Gönderen sizin adınıza gönderiyorsa, gönderenin IP adresini SPF kaydınıza ekleyerek bu adrese yetki vermeniz gerekir.
  
Daha [fazla bilgi için bkz. Dolandırıcılık algılaması için kırmızı (şüpheli) güvenlik](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) ipucu sorunlarını giderme.
  
Size yardımcı olacak diğer bazı bağlantılar:
  
- [Microsoft, sender Policy Framework'i (SPF) kullanarak kimliği doğrunlamayı önlemek için nasıl kullanır?](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF'yi, sanallık engellemeye yardımcı olacak şekilde ayarlama](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
