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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801095"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>SharePoint Online, OneDrive ve Microsoft ekipleri için Office 365 için Microsoft Defender 'ı etkinleştirme

1. Gidin https://protection.office.com ve oturum açın.
2. **Tehdit yönetimi**  >  **ilkesi**  >  **güvenli ekleri** 'ni seçin.
3. **SharePoint, OneDrive ve Microsoft ekipleri IÇIN ATP 'Yi aç** 'ı seçip **Kaydet** 'i tıklatın.
4. Öner Genel yönetici veya SharePoint Online yöneticisi olarak, [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet 'Ini **Disallowın, tedfiledownload** parametresini *true* olarak ayarlanmış şekilde çalıştırın.
5. Öner Algılanan dosyalar için [uyarıları ayarlayın](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) .

> [!NOTE]
> ATP, SharePoint Online, OneDrive veya Microsoft ekipte her dosyayı tarayacak. Dosyalar, paylaşım ve konuk etkinliği olaylarını kullanan bir süreç aracılığıyla, kötü amaçlı dosyaları tanımlayan akıllı buluşsal yöntemleri ve tehdit sinyalleriyle birlikte zaman uyumsuz olarak taranır. [SharePoint, OneDrive ve Microsoft ekipleri Için ATP 'yi](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)inceleyin.