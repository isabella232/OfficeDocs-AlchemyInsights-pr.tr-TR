---
title: Microsoft Defender ATP taraması için dışlamaları yapılandırma
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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "50714355"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="923c9-102">Microsoft Defender ATP taraması için dışlamaları yapılandırma</span><span class="sxs-lookup"><span data-stu-id="923c9-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="923c9-103">Genel olarak, belirli dosya uzantılarını ve klasör konumlarını Microsoft Defender ATP taramalarından çıkarabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="923c9-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="923c9-104">Belirli işlemlerle açılan dosyalar için dışlamaları da yapılandırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="923c9-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="923c9-105">Daha fazla bilgi için bkz. Dosya [uzantısına](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) ve klasör konumuna göre dışlamaları yapılandırma ve doğrulama ve süreçler tarafından açılan dosyalar için [dışlamaları yapılandırma.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="923c9-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="923c9-106">**Windows Server 2016 ve 2019'da** dışlamaları yapılandırmak için bkz. [Windows Server'da Microsoft Defender Virüsten Koruma dışlamalarını yapılandırma.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="923c9-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="923c9-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="923c9-107">**Mac**</span></span>

<span data-ttu-id="923c9-108">Desteklenen dışlama türleri ve Mac için dışlama listesini yapılandırma [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) hakkında ayrıntılı bilgi için, desteklenen dışlama türleri ve dışlama listesini [yapılandırma.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="923c9-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="923c9-109">**Not** Ayrıca, EICAR test dosyasını kullanarak dışlama listelerini doğrulaabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="923c9-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="923c9-110">Daha fazla bilgi için bkz. [EICAR test dosyasıyla dışlama listelerini doğrulama.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="923c9-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="923c9-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="923c9-111">**Linux**</span></span>

<span data-ttu-id="923c9-112">Desteklenen dışlama türleri ve Linux için dışlama listesini yapılandırma [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) hakkında ayrıntılı bilgi için, Desteklenen dışlama türlerine bakın ve Linux için [Microsoft Defender ATP'de](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)dışlamaları yapılandırma ve doğrulama.</span><span class="sxs-lookup"><span data-stu-id="923c9-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="923c9-113">**Not** Ayrıca, EICAR test dosyasını kullanarak dışlama listelerini doğrulaabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="923c9-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="923c9-114">Daha fazla bilgi için bkz. [EICAR test dosyasıyla dışlama listelerini doğrulama.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="923c9-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 