---
title: Dolandırıcılık algılama güvenlik ipucu sorunları giderme
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
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955986"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Dolandırıcılık algılama güvenlik ipucu sorunları giderme

"Gönderen, dolandırıcılık algılama güvenlik ipucu" ifadesinin bulunduğu bir e-posta alıyorsanız, gönderen DKIM veya SPF kimlik doğrulama denetimlerinden geçiremedi. Bunu çözmek için en iyi yöntem, gönderenin kendi yetkilerini vermesidir. Gönderen sizin adınıza gönderiyorsa, gönderenin IP adresini SPF kaydınıza ekleyerek bu adrese yetki vermeniz gerekir.
  
Daha [fazla bilgi için bkz. Kırmızı (şüpheli) güvenlik ipucu dolandırıcılık algılama denetimleri](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) için sorun giderme.
  
Size yardımcı olacak diğer bazı bağlantılar:
  
- [Microsoft, sender Policy Framework'i (SPF) kullanarak kimliği doğrunlamayı önlemek için nasıl kullanır?](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF'yi, sanallık engellemeye yardımcı olacak şekilde ayarlama](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
