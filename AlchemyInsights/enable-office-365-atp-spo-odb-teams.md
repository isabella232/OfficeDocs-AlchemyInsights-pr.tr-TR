---
title: SharePoint, OneDrive ve Microsoft ekipleri için Office 365 ATP 'yi etkinleştirme
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709927"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>SharePoint Online, OneDrive ve Microsoft ekipleri için Office 365 Gelişmiş tehdit korumasını etkinleştirme

1. Gidin https://protection.office.com ve oturum açın.
2. **Tehdit yönetimi**  >  **ilkesi**  >  **güvenli ekleri**'ni seçin.
3. **SharePoint, OneDrive ve Microsoft ekipleri IÇIN ATP 'Yi aç**'ı seçip **Kaydet**'i tıklatın.
4. Öner Genel yönetici veya SharePoint Online yöneticisi olarak, [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet 'Ini **Disallowın, tedfiledownload** parametresini *true*olarak ayarlanmış şekilde çalıştırın.
5. Öner Algılanan dosyalar için [uyarıları ayarlayın](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) .

> [!NOTE]
> ATP, SharePoint Online, OneDrive veya Microsoft ekipte her dosyayı tarayacak. Dosyalar, paylaşım ve konuk etkinliği olaylarını kullanan bir süreç aracılığıyla, kötü amaçlı dosyaları tanımlayan akıllı buluşsal yöntemleri ve tehdit sinyalleriyle birlikte zaman uyumsuz olarak taranır. [SharePoint, OneDrive ve Microsoft ekipleri Için ATP 'yi](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)inceleyin.