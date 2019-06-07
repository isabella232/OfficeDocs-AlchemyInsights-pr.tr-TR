---
title: SharePoint, OneDrive ve Microsoft ekipleri KM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: b304f6c7d9959e49a8152c03f11c6c864a154ea5
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765498"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="03c9c-102">SharePoint, OneDrive ve Microsoft ekipleri KM</span><span class="sxs-lookup"><span data-stu-id="03c9c-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="03c9c-103">Gelişmiş tehdidi korumasını etkinleştirmek için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="03c9c-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="03c9c-104">Git [https://protection.office.com](https://protection.office.com) ve genel yönetici veya güvenlik yöneticisi hesabı ile oturum açın.</span><span class="sxs-lookup"><span data-stu-id="03c9c-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="03c9c-105">**İlke** **tehdit Yönetimi**altında sol gezinti bölmesinde seçin \> **Güvenli ekler**.</span><span class="sxs-lookup"><span data-stu-id="03c9c-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="03c9c-106">**SharePoint, OneDrive, ve Microsoft ekipleri KM Aç**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="03c9c-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="03c9c-107">Biz kötü amaçlı dosyalar algıladıklarında bildirimleri almak için [bir etkinlik uyarı ilkesi oluşturun](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) .</span><span class="sxs-lookup"><span data-stu-id="03c9c-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="03c9c-108">Bu [konuda](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams)eksiksiz yönergeler için bkz.</span><span class="sxs-lookup"><span data-stu-id="03c9c-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="03c9c-109">**Not**: tasarım gereği, ATP her tek dosyada SharePoint çevrimiçi, OneDrive iş veya Microsoft Teams taramaz.</span><span class="sxs-lookup"><span data-stu-id="03c9c-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="03c9c-110">Dosya paylaşım etkinliği, Konuk etkinlik kullanan bir işlemin zaman uyumsuz olarak taranır ve kötü amaçlı dosyaları tanımlamak tehlike sinyalleri.</span><span class="sxs-lookup"><span data-stu-id="03c9c-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="03c9c-111">Bu [konuda](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="03c9c-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
