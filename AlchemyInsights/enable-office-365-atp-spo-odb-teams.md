---
title: SharePoint, OneDrive ve takımlar Microsoft Office 365 KM etkinleştir
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403053"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Çevrimiçi SharePoint, OneDrive ve takımlar Microsoft Office 365 Gelişmiş tehdit korumayı etkinleştir

1. Git https://protection.office.com ve oturum açın.
2. **Tehdit Yönetimi**seçin > **ilke** > **Güvenli ekler**.
3. **SharePoint, OneDrive, ve Microsoft ekipleri KM Aç**' ı seçin ve **Kaydet**' i tıklatın.
4. (Önerilen) Genel yönetici veya çevrimiçi SharePoint Yöneticisi **DisallowInfectedFileDownload** parametresi *doğru*ayarlanmış [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet'ini çalıştırın.
5. (Önerilen) [Uyarıları ayarlamak](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) için algılanan dosyaları.

> [!NOTE]
> ATP nBaşka tarama her tek dosyada SharePoint çevrimiçi, OneDrive veya Microsoft Teams olur. Dosyaları paylaşma ve Konuk etkinlik olaylarını, akıllı buluşsallık ve kötü amaçlı dosyaları tanımlamak için tehlike sinyalleri ile birlikte kullanan bir işlem üzerinden zaman uyumsuz olarak taranır. Bkz: [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).