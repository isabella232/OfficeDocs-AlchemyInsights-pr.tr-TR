---
title: Uç Noktalar için Microsoft Defender'a yerleştirme makineleri ile ilgili sorunlar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901587"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="4b203-102">Uç Noktalar için Microsoft Defender'a yerleştirme makineleri ile ilgili sorunlar</span><span class="sxs-lookup"><span data-stu-id="4b203-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="4b203-103">Makinelerin MDE hizmetine alınmasıyla ilgili sorunlarınız olabilir.</span><span class="sxs-lookup"><span data-stu-id="4b203-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="4b203-104">Son kullanıcı makinesine erişebiliyorsanız, şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="4b203-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="4b203-105">[MDE Client Analyzer](https://aka.ms/betamdeanalyzer) tanılama aracının en son önizleme sürümünü indirin.</span><span class="sxs-lookup"><span data-stu-id="4b203-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="4b203-106">**MDEClientAnalyzer.cmd**'ye sağ tıklayın ve "Yönetici olarak çalıştır" ı seçin.</span><span class="sxs-lookup"><span data-stu-id="4b203-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="4b203-107">**MDEClientAnalyzer.htm**'de önerilen herhangi bir kılavuza uyun.</span><span class="sxs-lookup"><span data-stu-id="4b203-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="4b203-108">Daha ayrıntılı günlükler için, **MDEClientAnalyzerResult** adlı oluşturulan alt klasörü inceleyin.</span><span class="sxs-lookup"><span data-stu-id="4b203-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="4b203-109">Ek yönlendirme gerekiyorsa, [Uç Nokta desteği için Microsoft Defender](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support)'a başvurun ve analiz için elde edilen MDEClientAnalyzerResult.zip dosyasını sağlayın.</span><span class="sxs-lookup"><span data-stu-id="4b203-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
