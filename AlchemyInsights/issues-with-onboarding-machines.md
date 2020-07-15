---
title: Onboarding makineleri ile ilgili sorunlar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141838"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="afd84-102">Onboarding makineleri ile ilgili sorunlar</span><span class="sxs-lookup"><span data-stu-id="afd84-102">Issues with onboarding machines</span></span>

<span data-ttu-id="afd84-103">MDATP hizmetine onboarding makineleri ile ilgili sorunlar olabilir.</span><span class="sxs-lookup"><span data-stu-id="afd84-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="afd84-104">Son kullanıcı makinesine erişebiliyorsanız, aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="afd84-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="afd84-105">[İstemci Bağlantı Çözümleyicisi](https://aka.ms/mdatpanalyzer) tanı aracını indirin.</span><span class="sxs-lookup"><span data-stu-id="afd84-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="afd84-106">Ayıklayın ve MDATPAnalyzer.cmd çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="afd84-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="afd84-107">Analyzer aracının indirildiği klasör olan MDATPClientAnalyzerResult adlı klasördeki tanılama günlüğünü bulun.</span><span class="sxs-lookup"><span data-stu-id="afd84-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="afd84-108">Bağlantı veya internet proxy ayarları sorunlarını bulmak için günlük dosyasını MDATPClientAnalyzer.txt gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="afd84-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>