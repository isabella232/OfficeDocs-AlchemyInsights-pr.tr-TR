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
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="eefd9-102">SharePoint Online, OneDrive ve Microsoft Ekipleri için Office 365 Gelişmiş Tehdit Koruması'nı etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="eefd9-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="eefd9-103">Git https://protection.office.com ve oturum aç.</span><span class="sxs-lookup"><span data-stu-id="eefd9-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="eefd9-104">**Tehdit yönetimi** > **Ilkesi** > **Güvenli Ekleri**seçin.</span><span class="sxs-lookup"><span data-stu-id="eefd9-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="eefd9-105">**SharePoint, OneDrive ve Microsoft Teams için ATP'yi aç'ı**seçin ve ardından **Kaydet'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="eefd9-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="eefd9-106">(Tavsiye edilir) Global bir yönetici veya SharePoint Online yöneticisi olarak, **DisallowInfectedFileDownload** parametresini *doğru*olarak ayarlı setile [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet'i çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="eefd9-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="eefd9-107">(Tavsiye edilir) Algılanan dosyalar için [uyarılar ayarlayın.](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)</span><span class="sxs-lookup"><span data-stu-id="eefd9-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="eefd9-108">ATP, SharePoint Online, OneDrive veya Microsoft Teams'deki her bir dosyayı taramaz.</span><span class="sxs-lookup"><span data-stu-id="eefd9-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="eefd9-109">Dosyalar, kötü amaçlı dosyaları tanımlamak için akıllı sezgisel ve tehdit sinyallerinin yanı sıra paylaşım ve konuk etkinlik etkinliklerini kullanan bir işlem aracılığıyla eş senkronize olarak taranır.</span><span class="sxs-lookup"><span data-stu-id="eefd9-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="eefd9-110">Bkz. [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="eefd9-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>