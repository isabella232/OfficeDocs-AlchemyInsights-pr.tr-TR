---
title: SharePoint, OneDrive ve Microsoft Ekipleri için Office 365 ATP'yi etkinleştirme
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703446"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>SharePoint Online, OneDrive ve Microsoft Ekipleri için Office 365 Gelişmiş Tehdit Koruması'nı etkinleştirme

1. Git https://protection.office.com ve oturum aç.
2. **Tehdit yönetimi** > **Ilkesi** > **Güvenli Ekleri**seçin.
3. **SharePoint, OneDrive ve Microsoft Teams için ATP'yi aç'ı**seçin ve ardından **Kaydet'i**tıklatın.
4. (Tavsiye edilir) Global bir yönetici veya SharePoint Online yöneticisi olarak, **DisallowInfectedFileDownload** parametresini *doğru*olarak ayarlı setile [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet'i çalıştırın.
5. (Tavsiye edilir) Algılanan dosyalar için [uyarılar ayarlayın.](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)

> [!NOTE]
> ATP, SharePoint Online, OneDrive veya Microsoft Teams'deki her bir dosyayı taramaz. Dosyalar, kötü amaçlı dosyaları tanımlamak için akıllı sezgisel ve tehdit sinyallerinin yanı sıra paylaşım ve konuk etkinlik etkinliklerini kullanan bir işlem aracılığıyla eş senkronize olarak taranır. Bkz. [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).