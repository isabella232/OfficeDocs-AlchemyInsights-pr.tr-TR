---
title: SharePoint, OneDrive için Office 365 için Microsoft Defender Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543597"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="87b76-102">SharePoint, OneDrive için Office 365 için Microsoft Defender Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="87b76-102">Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="87b76-103">Microsoft Defender for Office 365'u etkinleştirmek için şu Office 365:</span><span class="sxs-lookup"><span data-stu-id="87b76-103">Follow these steps to enable Microsoft Defender for Office 365:</span></span>

1. <span data-ttu-id="87b76-104">Genel yönetici [https://protection.office.com](https://protection.office.com) veya güvenlik yöneticisi hesabıyla gidin ve oturum açın.</span><span class="sxs-lookup"><span data-stu-id="87b76-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="87b76-105">Tehdit yönetimi altındaki sol gezinti bölmesinde **İlke ve**  \> **Ekler'i Kasa seçin.**</span><span class="sxs-lookup"><span data-stu-id="87b76-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="87b76-106">Office 365, **OneDrive ve SharePoint OneDrive için Defender'ı Microsoft Teams öğesini seçin.**</span><span class="sxs-lookup"><span data-stu-id="87b76-106">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="87b76-107">[Kötü amaçlı dosyalar algılayana](/microsoft-365/compliance/create-activity-alerts) kadar bildirim almak için bir etkinlik uyarısı ilkesi oluşturun.</span><span class="sxs-lookup"><span data-stu-id="87b76-107">[Create an activity alert policy](/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="87b76-108">Tüm yönergeler için bu [E-posta, Kasa, SharePoint, OneDrive için](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)Ekleri açma Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="87b76-108">For complete instructions, see this [Turn on Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="87b76-109">**Not:** Tasarım olarak, Office 365 için Microsoft Defender SharePoint Online, OneDrive İş veya Microsoft Teams'de tek tek dosyaları Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="87b76-109">**Note**: By design, Microsoft Defender for Office 365 doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="87b76-110">Dosyalar, kötü amaçlı dosyaları tanımlamak için paylaşım etkinliği, konuk etkinliği ve tehdit sinyallerini kullanan bir işlem tarafından zaman uyumsuz olarak taranır.</span><span class="sxs-lookup"><span data-stu-id="87b76-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="87b76-111">Daha fazla bilgi için [bkz. Kasa, Dosya SharePoint OneDrive ekleri Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="87b76-111">For more information, see [Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
