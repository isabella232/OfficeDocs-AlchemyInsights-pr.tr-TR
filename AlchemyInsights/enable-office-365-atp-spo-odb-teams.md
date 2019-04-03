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
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2019
ms.locfileid: "31031126"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="8bfa9-102">Çevrimiçi SharePoint, OneDrive ve takımlar Microsoft Office 365 Gelişmiş tehdit korumayı etkinleştir</span><span class="sxs-lookup"><span data-stu-id="8bfa9-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="8bfa9-103">Git https://protection.office.com ve oturum açın.</span><span class="sxs-lookup"><span data-stu-id="8bfa9-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="8bfa9-104">**Tehdit Yönetimi**seçin > **ilke** > **Güvenli ekler**.</span><span class="sxs-lookup"><span data-stu-id="8bfa9-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="8bfa9-105">**SharePoint, OneDrive, ve Microsoft ekipleri KM Aç**' ı seçin ve **Kaydet**' i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="8bfa9-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="8bfa9-106">(Önerilen) Genel yönetici veya çevrimiçi SharePoint Yöneticisi **DisallowInfectedFileDownload** parametresi *doğru*ayarlanmış [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet'ini çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="8bfa9-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="8bfa9-107">(Önerilen) [Uyarıları ayarlamak](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) için algılanan dosyaları.</span><span class="sxs-lookup"><span data-stu-id="8bfa9-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="8bfa9-108">ATP nBaşka tarama her tek dosyada SharePoint çevrimiçi, OneDrive veya Microsoft Teams olur.</span><span class="sxs-lookup"><span data-stu-id="8bfa9-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="8bfa9-109">Dosyaları paylaşma ve Konuk etkinlik olaylarını, akıllı buluşsallık ve kötü amaçlı dosyaları tanımlamak için tehlike sinyalleri ile birlikte kullanan bir işlem üzerinden zaman uyumsuz olarak taranır.</span><span class="sxs-lookup"><span data-stu-id="8bfa9-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="8bfa9-110">Bkz: [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="8bfa9-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>