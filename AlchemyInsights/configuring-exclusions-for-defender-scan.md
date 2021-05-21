---
title: Dışlamaları Microsoft Defender ATP yapılandırma
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543705"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="55d39-102">Dışlamaları Microsoft Defender ATP yapılandırma</span><span class="sxs-lookup"><span data-stu-id="55d39-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="55d39-103">Genelde, belirli dosya uzantılarını ve klasör konumlarını taramaların dışında Microsoft Defender ATP tutabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="55d39-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="55d39-104">Belirli işlemlerle açılan dosyalar için dışlamaları da yapılandırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="55d39-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="55d39-105">Daha fazla bilgi için bkz. [Dosya](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) uzantısını ve klasör konumunu temel alarak dışlamaları yapılandırma ve doğrulama ve İşlemler tarafından açılan dosyalar için [dışlamaları yapılandırma](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="55d39-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="55d39-106">**Windows Server 2016 2019'da dışlamaları** yapılandırmak için bkz. [Microsoft Defender Virüsten Koruma sunucusunda dışlamaları yapılandırma Windows](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="55d39-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="55d39-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="55d39-107">**Mac**</span></span>

<span data-ttu-id="55d39-108">Desteklenen dışlama türleri ve Mac için dışlama listesi yapılandırma [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) hakkında ayrıntılar için bkz. Desteklenen dışlama türleri ve Dışlama listesi [yapılandırma.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="55d39-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="55d39-109">**Not** Ayrıca EICAR test dosyasını kullanarak dışlama listelerini doğrulaabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="55d39-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="55d39-110">Daha fazla bilgi için [bkz. EICAR test dosyasıyla dışlama listelerini doğrulama.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="55d39-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="55d39-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="55d39-111">**Linux**</span></span>

<span data-ttu-id="55d39-112">Desteklenen dışlama türleri ve Linux için dışlamaların listesi [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) yapılandırma hakkında ayrıntılar için bkz. Desteklenen dışlama türleri ve Linux için dışlamaları yapılandırma [Microsoft Defender ATP doğrulama](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="55d39-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="55d39-113">**Not** Ayrıca EICAR test dosyasını kullanarak dışlama listelerini doğrulaabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="55d39-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="55d39-114">Daha fazla bilgi için [bkz. EICAR test dosyasıyla dışlama listelerini doğrulama.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="55d39-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 