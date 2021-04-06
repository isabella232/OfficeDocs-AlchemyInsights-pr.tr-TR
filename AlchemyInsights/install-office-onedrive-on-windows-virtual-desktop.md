---
title: Office ve OneDrive'ı Windows Sanal Masaüstü'ne yükleme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596030"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="375d7-102">Office ve OneDrive'ı Windows Sanal Masaüstü'ne yükleme</span><span class="sxs-lookup"><span data-stu-id="375d7-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="375d7-103">[Asıl VHD görüntüsünü hazırlama ve özelleştirme.](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image)</span><span class="sxs-lookup"><span data-stu-id="375d7-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="375d7-104">Henüz oluşturulmamış bir sanal makine (VM) oluşturun.</span><span class="sxs-lookup"><span data-stu-id="375d7-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="375d7-105">[Office'i paylaşılan bilgisayar etkinleştirme modunda yükleyin.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)</span><span class="sxs-lookup"><span data-stu-id="375d7-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="375d7-106">Paylaşılan bilgisayar etkinleştirmesi, birden çok kullanıcının Office'e erişmelerine olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="375d7-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="375d7-107">[OneDrive'ı makine başına modda yükleyin.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)</span><span class="sxs-lookup"><span data-stu-id="375d7-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="375d7-108">Normalde, OneDrive kullanıcı başına yüklenir, ancak burada her makineye yüklenmiş olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="375d7-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>