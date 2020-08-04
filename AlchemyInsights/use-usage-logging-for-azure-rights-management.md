---
title: Azure Hakları Yönetimi için kullanım günlüğü kullanma
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5506"
- "9002281"
ms.openlocfilehash: 606fcdc5394edab26c60925af28cf2d938aac172
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/03/2020
ms.locfileid: "46556025"
---
# <a name="use-usage-logging-for-azure-rights-management"></a><span data-ttu-id="8e5e0-102">Azure Hakları Yönetimi için kullanım günlüğü kullanma</span><span class="sxs-lookup"><span data-stu-id="8e5e0-102">Use usage logging for Azure Rights Management</span></span>

<span data-ttu-id="8e5e0-103">Varsayılan olarak, koruma kullanım günlüğü tüm müşteriler için etkinleştirilir.</span><span class="sxs-lookup"><span data-stu-id="8e5e0-103">By default, protection usage logging is enabled for all customers.</span></span> <span data-ttu-id="8e5e0-104">Günlükler, kiracınız için Azure depolama alanında bir dizi blob olarak yazılır.</span><span class="sxs-lookup"><span data-stu-id="8e5e0-104">Logs are written as a series of blobs in Azure storage for your tenant.</span></span> <span data-ttu-id="8e5e0-105">Koruma eyleminden sonra, günlüklerin çoğunun görünmesi 15 dakika kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="8e5e0-105">After a protection action, it might take up to 15 minutes for most logs to appear.</span></span>

<span data-ttu-id="8e5e0-106">Koruma kullanım günlüklerini şu şekilde kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="8e5e0-106">You can use protection usage logs to:</span></span>

- <span data-ttu-id="8e5e0-107">İş öngörülerini analiz edin</span><span class="sxs-lookup"><span data-stu-id="8e5e0-107">Analyze business insights</span></span>

- <span data-ttu-id="8e5e0-108">Kötüye kullanım için monitör</span><span class="sxs-lookup"><span data-stu-id="8e5e0-108">Monitor for abuse</span></span>

- <span data-ttu-id="8e5e0-109">Adli analiz yapın</span><span class="sxs-lookup"><span data-stu-id="8e5e0-109">Perform forensic analysis</span></span>

<span data-ttu-id="8e5e0-110">Daha fazla bilgi için Bkz. [Azure Bilgi Koruması'ndan koruma kullanımını günlüğe kaydetme ve çözümleme.](https://docs.microsoft.com/azure/information-protection/log-analyze-usage)</span><span class="sxs-lookup"><span data-stu-id="8e5e0-110">For more information, see [Logging and analyzing the protection usage from Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span></span>

<span data-ttu-id="8e5e0-111">İstemci kullanımı günlüğe kaydetme hakkında daha fazla bilgi için Bkz. [Yönetici Kılavuzu: Azure Bilgi Koruması istemci dosyaları ve istemci kullanımı günlüğü.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging)</span><span class="sxs-lookup"><span data-stu-id="8e5e0-111">For information about client usage logging, see [Admin Guide: Azure Information Protection client files and client usage logging](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span></span>

<span data-ttu-id="8e5e0-112">Daha fazla bilgi için bkz:</span><span class="sxs-lookup"><span data-stu-id="8e5e0-112">For additional information, see:</span></span>

- <span data-ttu-id="8e5e0-113">[Azure Bilgi Koruması gereksinimleri.](https://docs.microsoft.com/azure/information-protection/get-started/requirements)</span><span class="sxs-lookup"><span data-stu-id="8e5e0-113">[Azure Information Protection requirements](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span></span>
    
- <span data-ttu-id="8e5e0-114">[Öğretici: Azure Bilgi Koruma ilkesi ayarlarını yapılandırın ve yeni bir etiket oluşturun.](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)</span><span class="sxs-lookup"><span data-stu-id="8e5e0-114">[Tutorial: Configure Azure Information Protection policy settings and create a new label](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span></span>