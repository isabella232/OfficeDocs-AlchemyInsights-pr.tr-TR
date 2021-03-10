---
title: Mac'te MDATP yükleme sorunlarını giderme
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696099"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="1f6bd-102">Mac'te MDATP yükleme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="1f6bd-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="1f6bd-103">El ile yükleme başarısız **olursa, yükleme** sihirbazının Özet sayfası aşağıdaki hatayı gösterir:</span><span class="sxs-lookup"><span data-stu-id="1f6bd-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="1f6bd-104">"Yükleme sırasında bir hata oluştu.</span><span class="sxs-lookup"><span data-stu-id="1f6bd-104">"An error occurred during installation.</span></span> <span data-ttu-id="1f6bd-105">Yükleyici, yüklemenin başarısız olmasına neden olan bir hatayla karşılaştı.</span><span class="sxs-lookup"><span data-stu-id="1f6bd-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="1f6bd-106">Yardım için yazılım üreticisine başvurun."</span><span class="sxs-lookup"><span data-stu-id="1f6bd-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="1f6bd-107">MDM dağıtımları için, sayfada genel yükleme hatası da görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="1f6bd-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="1f6bd-108">Son kullanıcılara tam hatalar görüntülense de, **/Library/Logs/Microsoft/mdatp/install.log** dosyasında yükleme ilerlemesi olan bir günlük dosyası tutabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1f6bd-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="1f6bd-109">Her yükleme oturumu bu günlük dosyasının sonuna eklenir.</span><span class="sxs-lookup"><span data-stu-id="1f6bd-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="1f6bd-110">Yalnızca son yükleme oturumunun çıkışını yapmak için `sed` kullanın.</span><span class="sxs-lookup"><span data-stu-id="1f6bd-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="1f6bd-111">Daha fazla bilgi edinmek için [Mac için Microsoft Defender ATP'de yükleme sorunlarını giderme makalesine bakın.](https://go.microsoft.com/fwlink/?linkid=2144615)</span><span class="sxs-lookup"><span data-stu-id="1f6bd-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
