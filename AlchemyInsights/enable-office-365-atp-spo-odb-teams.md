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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709927"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="52e12-102">SharePoint Online, OneDrive ve Microsoft ekipleri için Office 365 Gelişmiş tehdit korumasını etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="52e12-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="52e12-103">Gidin https://protection.office.com ve oturum açın.</span><span class="sxs-lookup"><span data-stu-id="52e12-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="52e12-104">**Tehdit yönetimi**  >  **ilkesi**  >  **güvenli ekleri**'ni seçin.</span><span class="sxs-lookup"><span data-stu-id="52e12-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="52e12-105">**SharePoint, OneDrive ve Microsoft ekipleri IÇIN ATP 'Yi aç**'ı seçip **Kaydet**'i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="52e12-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="52e12-106">Öner Genel yönetici veya SharePoint Online yöneticisi olarak, [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet 'Ini **Disallowın, tedfiledownload** parametresini *true*olarak ayarlanmış şekilde çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="52e12-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="52e12-107">Öner Algılanan dosyalar için [uyarıları ayarlayın](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) .</span><span class="sxs-lookup"><span data-stu-id="52e12-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="52e12-108">ATP, SharePoint Online, OneDrive veya Microsoft ekipte her dosyayı tarayacak.</span><span class="sxs-lookup"><span data-stu-id="52e12-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="52e12-109">Dosyalar, paylaşım ve konuk etkinliği olaylarını kullanan bir süreç aracılığıyla, kötü amaçlı dosyaları tanımlayan akıllı buluşsal yöntemleri ve tehdit sinyalleriyle birlikte zaman uyumsuz olarak taranır.</span><span class="sxs-lookup"><span data-stu-id="52e12-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="52e12-110">[SharePoint, OneDrive ve Microsoft ekipleri Için ATP 'yi](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)inceleyin.</span><span class="sxs-lookup"><span data-stu-id="52e12-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>