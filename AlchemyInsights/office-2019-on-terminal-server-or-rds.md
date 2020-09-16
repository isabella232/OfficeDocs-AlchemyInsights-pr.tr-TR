---
title: Terminal Server veya RDS üzerinde Office 2019
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3487"
- "9001419"
ms.openlocfilehash: 5454fad58411e9d86e19dfa83a1a553a2c2b05b4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47754585"
---
# <a name="deploying-office-2019-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="92bb7-102">RDS, Terminal Server veya VDı 'da Office 2019 ' i paylaşılan kullanıma dağıtma</span><span class="sxs-lookup"><span data-stu-id="92bb7-102">Deploying Office 2019 for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="92bb7-103">Office, başka herhangi bir Office planını kullanan RDS sunucusunda zaten yüklüyse kaldırın.</span><span class="sxs-lookup"><span data-stu-id="92bb7-103">If Office is already installed on the RDS server using any other Office plans, uninstall it.</span></span> <span data-ttu-id="92bb7-104">Örneğin, **Denetim Masası**'na gidin  >  **Uninstall a program**.</span><span class="sxs-lookup"><span data-stu-id="92bb7-104">For example, go to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="92bb7-105">Sorunlarla karşılaşıyorsanız, [Microsoft destek ve Kurtarma Yardımcısı 'nı](https://aka.ms/SARA-OfficeUninstall-Alchemy)kullanarak kaldırın.</span><span class="sxs-lookup"><span data-stu-id="92bb7-105">If you're experiencing issues, uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy).</span></span> 

<span data-ttu-id="92bb7-106">Office 'i yüklemek için Office dağıtım aracı 'nı (ODT) kullanın.</span><span class="sxs-lookup"><span data-stu-id="92bb7-106">Use the Office Deployment Tool (ODT) to install Office.</span></span> <span data-ttu-id="92bb7-107">Ayrıntılı adımlar için [Office 2019 'ı dağıtma](https://docs.microsoft.com/deployoffice/office2019/deploy)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="92bb7-107">For detailed steps, see [Deploy Office 2019](https://docs.microsoft.com/deployoffice/office2019/deploy).</span></span>

<span data-ttu-id="92bb7-108">Etkinleştirme için, [Office 'in toplu etkinleştirme konusuna genel bakış](https://docs.microsoft.com/deployoffice/vlactivation/plan-volume-activation-of-office)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="92bb7-108">For activation, see [Overview of volume activation of Office](https://docs.microsoft.com/deployoffice/vlactivation/plan-volume-activation-of-office).</span></span>