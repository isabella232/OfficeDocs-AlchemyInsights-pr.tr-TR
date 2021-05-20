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
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="cb7a9-102">SharePoint Online, OneDrive ve Office 365 için Microsoft Defender'ı Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="cb7a9-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="cb7a9-103">Gidin https://protection.office.com ve oturum açma.</span><span class="sxs-lookup"><span data-stu-id="cb7a9-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="cb7a9-104">Ekleri **Tehdit Yönetimi**  >  **İlkesi**  >  **Kasa seçin.**</span><span class="sxs-lookup"><span data-stu-id="cb7a9-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="cb7a9-105">SharePoint, **OneDrive ve Microsoft Teams için Office 365 Defender'ı aç'ı** seçin ve kaydet'e **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="cb7a9-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="cb7a9-106">(Önerilen) Genel yönetici veya SharePoint Online yöneticisi olarak [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet'ini **DisallowInfectedFileDownload** parametresi true olarak *ayarlanmış olarak çalıştırın.*</span><span class="sxs-lookup"><span data-stu-id="cb7a9-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="cb7a9-107">(Önerilen) [Algılanan dosyalar için](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) uyarılar ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="cb7a9-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="cb7a9-108">Office 365 için Microsoft Defender, SharePoint Online, OneDrive veya Microsoft Teams'de tek tek dosyaları taramaz.</span><span class="sxs-lookup"><span data-stu-id="cb7a9-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="cb7a9-109">Dosyalar zaman uyumsuz olarak, kötü amaçlı dosyaları tanımlamak için akıllı heuristler ve tehdit işaretleriyle birlikte paylaşım ve konuk etkinliği olaylarını kullanan bir işlem aracılığıyla taranır.</span><span class="sxs-lookup"><span data-stu-id="cb7a9-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="cb7a9-110">Bkz. [Office 365, SharePoint için Microsoft Defender OneDrive ve Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="cb7a9-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>