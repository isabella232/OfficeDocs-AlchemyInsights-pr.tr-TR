---
title: OFFICE 365, ONEDRIVE ve SharePoint için ATP'yi Microsoft Teams
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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543948"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>SharePoint Online, OneDrive ve Office 365 için Microsoft Defender'ı Microsoft Teams

1. Gidin https://protection.office.com ve oturum açma.
2. Ekleri **Tehdit Yönetimi**  >  **İlkesi**  >  **Kasa seçin.**
3. SharePoint, **OneDrive ve Microsoft Teams için Office 365 Defender'ı aç'ı** seçin ve kaydet'e **tıklayın.**
4. (Önerilen) Genel yönetici veya SharePoint Online yöneticisi olarak [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet'ini **DisallowInfectedFileDownload** parametresi true olarak *ayarlanmış olarak çalıştırın.*
5. (Önerilen) [Algılanan dosyalar için](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) uyarılar ayarlayın.

> [!NOTE]
> Office 365 için Microsoft Defender, SharePoint Online, OneDrive veya Microsoft Teams'de tek tek dosyaları taramaz. Dosyalar zaman uyumsuz olarak, kötü amaçlı dosyaları tanımlamak için akıllı heuristler ve tehdit işaretleriyle birlikte paylaşım ve konuk etkinliği olaylarını kullanan bir işlem aracılığıyla taranır. Bkz. [Office 365, SharePoint için Microsoft Defender OneDrive ve Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)