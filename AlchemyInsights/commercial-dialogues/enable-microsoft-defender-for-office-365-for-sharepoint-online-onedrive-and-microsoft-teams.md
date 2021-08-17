---
title: SharePoint Online, E-posta Kasa Için Ekleri OneDrive Etkinleştirme Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894483"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>SharePoint Online, E-posta Kasa Için Ekleri OneDrive Etkinleştirme Microsoft Teams

1. Genel yönetici veya güvenlik yöneticisi kimlik bilgilerinizi kullanarak Microsoft 365 Defender portalını açın ve ardından İlkeler & kuralları tehdit ilkeleri ve İlkeler bölümünde Kasa ekleri'ne <https://security.microsoft.com>  \>  \>  gidin 

   Ekler sayfasında doğrudan **Kasa için,** <https://security.microsoft.com/safeattachmentv2> kullanın.

2. Ekler **Kasa Genel** ayarlar'a **tıklayın.**
3. Görüntülenen açılır çıktıda, SharePoint, OneDrive ve Office 365 için **Microsoft Defender'ı** Microsoft Teams ve ardından Kaydet'i **seçin.**

    > [!TIP]
    >
    > E-posta ekleri, ekleri Kasa için SharePoint geliştirmek OneDrive adımları Microsoft Teams:
    >
    > - Kullanıcıların kötü amaçlı dosyaları indirmesini önlemek için, `$true` SharePoint Online PowerShell'de **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** cmdlet'inin *DisallowInfectedFileDownload* parametresinin değerini kullanın. Daha fazla bilgi için bkz. SharePoint kötü amaçlı [dosyaları indirmelerini engellemek için SharePoint Online PowerShell kullanma](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files).
    > - [Algılanan dosyalar için uyarı ilkesi oluşturma](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Daha fazla bilgi için [bkz. Kasa, Dosya ve Office 365 için SharePoint OneDrive. Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
