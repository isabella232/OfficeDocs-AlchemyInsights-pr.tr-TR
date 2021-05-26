---
title: Uç nokta DLP’sini yapılandırma
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657949"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="7b49b-102">Uç nokta DLP’sini yapılandırma</span><span class="sxs-lookup"><span data-stu-id="7b49b-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="7b49b-103">Microsoft Uç nokta DLP’si, Windows 10 cihazlarında DLP koruma ve izleme özelliğini hassas bilgilere kadar genişletmenize olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="7b49b-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="7b49b-104">Cihazlar cihaz yönetimine eklendikten sonra, öğeler üzerinde koruyucu eylemler uygulamak amacıyla DLP ilkeleri oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7b49b-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="7b49b-105">Hassas öğelerle ilgili etkinlikleri izlemek için Etkinlik Gezgini kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="7b49b-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="7b49b-106">Daha fazla bilgi için bkz. [Cihazları cihaz yönetimine ekleme](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="7b49b-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="7b49b-107">Uç nokta DLP’sini kullanmaya başlamak için:</span><span class="sxs-lookup"><span data-stu-id="7b49b-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="7b49b-108">Uygun SKU/abonelik lisansına sahip olduğunuzdan emin olun.</span><span class="sxs-lookup"><span data-stu-id="7b49b-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="7b49b-109">Daha fazla bilgi için bkz. [SKU/abonelik lisansı](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="7b49b-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="7b49b-110">Cihaz yönetimini etkinleştirmek, katılım sayfasına erişmek veya cihaz izlemeyi etkinleştirmek/devre dışı bırakmak için gerekli izinleri kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="7b49b-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="7b49b-111">Daha fazla bilgi için bkz. [İzinler](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="7b49b-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="7b49b-112">Aşağıdaki cihaz ekleme yordamını izleyerek cihazları Cihaz yönetimine ekleyin.</span><span class="sxs-lookup"><span data-stu-id="7b49b-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="7b49b-113">Daha fazla bilgi için bkz. [Cihazları ekleme](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="7b49b-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="7b49b-114">Hassas öğelerinizi korumak için DLP ilkeleri oluşturun.</span><span class="sxs-lookup"><span data-stu-id="7b49b-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="7b49b-115">Bilgi için bkz. [Uç nokta DLP ilkesi senaryoları](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="7b49b-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="7b49b-116">Microsoft Uç nokta DLP’si hakkında daha fazla bilgi için bkz. [Microsoft 365 uç noktada veri kaybını önleme (önizleme) özelliği hakkında bilgi edinin](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="7b49b-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="7b49b-117">**Destek gerekirse, Önemli Veri Toplama adımları:**</span><span class="sxs-lookup"><span data-stu-id="7b49b-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="7b49b-118">İstemci [Çözümleyicisi MDATP Önizlemesi'ne indirin.](https://aka.ms/betamdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="7b49b-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="7b49b-119">Aracı cmd penceresinden Yönetici olarak çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="7b49b-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="7b49b-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="7b49b-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="7b49b-121">İzlemeleri toplamak **için dakika sayısını girin:** ile sorulsa, senaryoyu çalıştırmak için gereken dakika sayısını girin.</span><span class="sxs-lookup"><span data-stu-id="7b49b-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="7b49b-122">Senaryoyu çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="7b49b-122">Run the scenario.</span></span>

<span data-ttu-id="7b49b-123">Destek temsilcisine vermek için Zip dosyası çıkışını toplayın.</span><span class="sxs-lookup"><span data-stu-id="7b49b-123">Collect the Zip file output to give to the Support agent.</span></span>
