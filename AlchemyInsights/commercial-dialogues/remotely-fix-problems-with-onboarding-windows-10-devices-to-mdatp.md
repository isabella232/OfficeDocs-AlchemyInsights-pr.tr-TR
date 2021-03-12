---
title: Windows 10 cihazlarını Microsoft Defender Gelişmiş Tehdit Koruması'ya eklemeyle ilgili sorunları uzaktan düzeltme
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750046"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="22e40-102">Windows 10 cihazlarını Microsoft Defender Gelişmiş Tehdit Koruması'ya eklemeyle ilgili sorunları uzaktan düzeltme</span><span class="sxs-lookup"><span data-stu-id="22e40-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="22e40-103">Uzak bilgisayara erişebilirsiniz, şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="22e40-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="22e40-104">İstemci Bağlantısı [Çözümleyicisi tanılama](https://go.microsoft.com/fwlink/?linkid=2143466) aracını indirin.</span><span class="sxs-lookup"><span data-stu-id="22e40-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="22e40-105">MDATPAnalyzer.cmd'yi ayıkla ve çalıştır.</span><span class="sxs-lookup"><span data-stu-id="22e40-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="22e40-106">Çözümleyici aracının indiriliş klasörüyle aynı klasör olan MDATPClientAnalyzerResult klasöründe tanılama günlüğünü bulun.</span><span class="sxs-lookup"><span data-stu-id="22e40-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="22e40-107">Bağlantı veya İnternet ara sunucusu ayarlarıyla ilgili sorunları bulmak için günlük dosyasını gözden MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="22e40-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="22e40-108">Daha fazla bilgi edinmek için, [işe alım makineleriyle ilgili sorunlar'a bakın.](https://go.microsoft.com/fwlink/?linkid=2143634)</span><span class="sxs-lookup"><span data-stu-id="22e40-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
