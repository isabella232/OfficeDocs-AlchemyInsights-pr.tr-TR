---
title: Teams'i Office yüklemelerinden kaldırma veya dışlama
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 2d96d54cb479f5f52cc707d4307cf9cf1e891a01
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827812"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="e54f7-102">Teams'i yeni veya mevcut Office yüklemelerinden kaldırma veya dışlama</span><span class="sxs-lookup"><span data-stu-id="e54f7-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="e54f7-103">Microsoft Teams; Kurumsal Microsoft 365 Uygulamaları, İş için Microsoft 365 Uygulamaları ve Mac için Office'in bir parçası olarak dahil edilir.</span><span class="sxs-lookup"><span data-stu-id="e54f7-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="e54f7-104">[Teams'i yeni Office yüklemelerinin](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) dışında tutmak için Office Dağıtım Aracı'nı kullanın.</span><span class="sxs-lookup"><span data-stu-id="e54f7-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="e54f7-105">*Teams'i* Windows çalıştıran bir cihazdan kaldırmak için bkz. [Microsoft Teams'i kaldırma.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)</span><span class="sxs-lookup"><span data-stu-id="e54f7-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="e54f7-106">Microsoft Teams'i birden çok hedef makine veya kullanıcıdan temizlemek için [bkz. Microsoft Teams dağıtımı temizleme.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)</span><span class="sxs-lookup"><span data-stu-id="e54f7-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="e54f7-107">Microsoft Teams'in Office ile otomatik olarak yüklemesini engellemek için [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) seçeneğini kullanın.</span><span class="sxs-lookup"><span data-stu-id="e54f7-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="e54f7-108">Microsoft Teams'in kurulumdan sonra otomatik olarak başlamasını önlemek için *Teams* yüklenmeden önce [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) seçeneğini kullanın.</span><span class="sxs-lookup"><span data-stu-id="e54f7-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="e54f7-109">Office Mac kullanıyorsanız bkz. [Mac'te Microsoft Teams yüklemeleri](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="e54f7-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>