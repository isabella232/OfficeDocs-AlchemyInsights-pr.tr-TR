---
title: Linux'ta Uç Nokta için Microsoft Defender performans sorunları
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794223"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="8d7c7-102">Linux'ta Uç Nokta için Microsoft Defender performans sorunları</span><span class="sxs-lookup"><span data-stu-id="8d7c7-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="8d7c7-103">Bu makale, Linux'ta Uç Nokta için Microsoft Defender performans sorunlarını belirleme adımsında size yol sunar.</span><span class="sxs-lookup"><span data-stu-id="8d7c7-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="8d7c7-104">Öncelikle, en son sürümle karşılaşan sorunun çözülmüş olduğunu [doğrulamanız önemlidir.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="8d7c7-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="8d7c7-105">Araştırmanızı başlatmak için bkz. [Linux'ta Uç Nokta için Microsoft Defender performans sorunlarını giderme.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="8d7c7-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="8d7c7-106">Dışlamalar</span><span class="sxs-lookup"><span data-stu-id="8d7c7-106">Exclusions</span></span>

<span data-ttu-id="8d7c7-107">Dışlamalar performans sorunlarının azaltmak için yardımcı olabilir.</span><span class="sxs-lookup"><span data-stu-id="8d7c7-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="8d7c7-108">Ek riskler bilindiği ve belgelenmiş olduğu için, başlamadan önce dışlamalarınızı gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8d7c7-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="8d7c7-109">Daha fazla bilgi için [bkz. Linux'ta Uç Nokta için Microsoft Defender için dışlamaları yapılandırma ve doğrulama.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="8d7c7-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="8d7c7-110">Dışlamak istediğiniz & çok dosya varsa ve hepsi aynı bağlama üzerinde olduğunda, bağlama klasörünü dışarıda tutmak daha kolay olabilir.</span><span class="sxs-lookup"><span data-stu-id="8d7c7-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="8d7c7-111">Şubat sürümü 101.22.80'den başlayarak tüm mountpoint'i dahil çekesiniz.</span><span class="sxs-lookup"><span data-stu-id="8d7c7-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="8d7c7-112">Örneğin, /mnt/backup bir mountpoint ise, şu komutu çalıştırarak dışlama listesine /mnt/backup ekleyebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="8d7c7-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="8d7c7-113">**Not:** Dışlamaların eklanması kötü amaçlı yazılım algılanma riskini artırır ve özenli bir şekilde ele geçiril olmalı ve uygulanmalı.</span><span class="sxs-lookup"><span data-stu-id="8d7c7-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="8d7c7-114">Yardıma mı ihtiyacınız var?</span><span class="sxs-lookup"><span data-stu-id="8d7c7-114">Need Help?</span></span>

<span data-ttu-id="8d7c7-115">Size en verimli şekilde yardımcı olmak için bir destek durumu açmadan önce tanılama verilerini toplayın.</span><span class="sxs-lookup"><span data-stu-id="8d7c7-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
