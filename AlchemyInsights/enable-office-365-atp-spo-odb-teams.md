---
title: Office 365 SHAREPOINT, ONEDRIVE ve SharePoint için ATP'yi Microsoft Teams
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
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332179"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>SharePoint Online, OneDrive ve diğer Office 365 için Microsoft Defender'ı Microsoft Teams

1. Gidin https://protection.office.com ve oturum açma.
2. Ekleri **Tehdit**  >  **Yönetimi İlkesi** Kasa  >  **seçin.**
3. SharePoint, **OneDrive ve Microsoft Teams için** defender Office 365'i seçin ve Kaydet'e **tıklayın.**
4. (Önerilen) Genel yönetici veya SharePoint Online yöneticisi olarak [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet'ini **DisallowInfectedFileDownload** parametresi true olarak ayarlanmış olarak *çalıştırın.*
5. (Önerilen) [Algılanan dosyalar için](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) uyarılar ayarlayın.

**Not:** Office 365 için Microsoft Defender SharePoint Online, OneDrive veya Microsoft Teams'te tek tek Microsoft Teams. Dosyalar zaman uyumsuz olarak, kötü amaçlı dosyaları tanımlamak için akıllı heuristler ve tehdit işaretleriyle birlikte paylaşım ve konuk etkinliği olaylarını kullanan bir işlem aracılığıyla taranır. SharePoint, [Office 365 OneDrive ve Microsoft Teams için Microsoft Defender'a Microsoft Teams.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)
