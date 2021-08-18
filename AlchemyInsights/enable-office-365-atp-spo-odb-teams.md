---
title: OFFICE 365, OneDrive ve SharePoint için ATP'yi Microsoft Teams
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
ms.openlocfilehash: 4a29fdf1b61dd51b85793a1346bea193c67f70d32344470cb5449cf767da4a24
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896623"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>SharePoint Online, OneDrive ve diğer Office 365 için Microsoft Defender'ı Microsoft Teams

1. Gidin https://protection.office.com ve oturum açma.
2. Ekleri **Tehdit yönetimi**  >  **İlkesi**  >  **Kasa seçin.**
3. SharePoint, **OneDrive ve Office 365 için Defender'ı Microsoft Teams'ı** seçin ve Kaydet'e **tıklayın.**
4. (Önerilen) Genel yönetici veya SharePoint Online yöneticisi olarak [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet'ini **DisallowInfectedFileDownload** parametresi true olarak *ayarlanmış olarak çalıştırın.*
5. (Önerilen) [Algılanan dosyalar için](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) uyarılar ayarlayın.

> [!NOTE]
> Office 365 için Microsoft Defender, SharePoint Online, OneDrive veya Microsoft Teams'de tek tek dosyaları taramaz. Dosyalar zaman uyumsuz olarak, kötü amaçlı dosyaları tanımlamak için akıllı heuristler ve tehdit işaretleriyle birlikte paylaşım ve konuk etkinliği olaylarını kullanan bir işlem aracılığıyla taranır. Bkz. [Office 365, SharePoint için Microsoft Defender OneDrive. Microsoft Teams.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)