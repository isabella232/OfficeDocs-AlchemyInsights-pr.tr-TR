---
title: SharePoint ve Office OneDrive'da dosya SharePoint duyarlılık etiketlerinin sınırlamaları
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813169"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>SharePoint ve Office OneDrive'da dosya SharePoint duyarlılık etiketlerinin sınırlamaları

SharePoint ve Office dosyaları için duyarlılık SharePoint OneDrive, gereksinimler ve sınırlamalara dikkat edin:

- SharePoint ve OneDrive dosyalar PowerQuery verileri, özel eklentiler tarafından depolanan veriler veya özel XML bölümleri içeriyorsa, Office masaüstü uygulamaları tarafından etiketlenmiş ve şifrelenmiş bazı dosyaları işleyememektedir.
- SharePoint ve OneDrive, Azure Information Protection (AIP) etiketlerini kullanarak zaten şifrelenmiş olan mevcut dosyalara otomatik olarak duyarlılık etiketleri uygulamaz. Şifreli dosyalara duyarlılık etiketleri uygulamak için: 
    - AIP etiketlerinin geçirilir ve Uyumluluk Merkezi'ne Microsoft 365 olun.
    - Etiketli dosyaları indirin ve özgün dosyalarına veya konumlarına SharePoint OneDrive yükleyin.
- Şifreli belgelerde yazdırma desteklenmemektedir.

Sınırlamalarla ilgili ek ayrıntılar için bkz. SharePoint ve Office dosyaları için [duyarlılık etiketlerini OneDrive.](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)
