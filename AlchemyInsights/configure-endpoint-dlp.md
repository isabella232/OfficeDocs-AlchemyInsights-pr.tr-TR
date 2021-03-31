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
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402463"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="572e2-102">Uç nokta DLP’sini yapılandırma</span><span class="sxs-lookup"><span data-stu-id="572e2-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="572e2-103">Microsoft Uç nokta DLP’si, Windows 10 cihazlarında DLP koruma ve izleme özelliğini hassas bilgilere kadar genişletmenize olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="572e2-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="572e2-104">Cihazlar cihaz yönetimine eklendikten sonra, öğeler üzerinde koruyucu eylemler uygulamak amacıyla DLP ilkeleri oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="572e2-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="572e2-105">Hassas öğelerle ilgili etkinlikleri izlemek için Etkinlik Gezgini kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="572e2-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="572e2-106">Daha fazla bilgi için bkz. [Cihazları cihaz yönetimine ekleme](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="572e2-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="572e2-107">Uç nokta DLP’sini kullanmaya başlamak için:</span><span class="sxs-lookup"><span data-stu-id="572e2-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="572e2-108">Uygun SKU/abonelik lisansına sahip olduğunuzdan emin olun.</span><span class="sxs-lookup"><span data-stu-id="572e2-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="572e2-109">Daha fazla bilgi için bkz. [SKU/abonelik lisansı](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="572e2-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="572e2-110">Cihaz yönetimini etkinleştirmek, katılım sayfasına erişmek veya cihaz izlemeyi etkinleştirmek/devre dışı bırakmak için gerekli izinleri kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="572e2-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="572e2-111">Daha fazla bilgi için bkz. [İzinler](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="572e2-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="572e2-112">Aşağıdaki cihaz ekleme yordamını izleyerek cihazları Cihaz yönetimine ekleyin.</span><span class="sxs-lookup"><span data-stu-id="572e2-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="572e2-113">M365 Uyumluluk **Ayarları** altında Cihaz Ekleme (önizleme) seçeneği bulunmuyorsa, yukarıda bahsedilen uygun lisansa ve izinlere sahip olduğunuzu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="572e2-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="572e2-114">Daha fazla bilgi için bkz. [Cihazları ekleme](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="572e2-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="572e2-115">Hassas öğelerinizi korumak için DLP ilkeleri oluşturun.</span><span class="sxs-lookup"><span data-stu-id="572e2-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="572e2-116">Bilgi için bkz. [Uç nokta DLP ilkesi senaryoları](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="572e2-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="572e2-117">Microsoft Uç nokta DLP’si hakkında daha fazla bilgi için bkz. [Microsoft 365 uç noktada veri kaybını önleme (önizleme) özelliği hakkında bilgi edinin](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="572e2-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="572e2-118">**Destek gerekirse, Önemli Veri Toplama adımları:**</span><span class="sxs-lookup"><span data-stu-id="572e2-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="572e2-119">MDATP Client Analyzer Preview aracını [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer") adresinden indirin</span><span class="sxs-lookup"><span data-stu-id="572e2-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="572e2-120">Aracı cmd penceresinden Yönetici olarak çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="572e2-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="572e2-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="572e2-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="572e2-122">“İzlemeleri toplamak için gereken dakika sayısını girin:” istemi göründüğünde, senaryoyu çalıştırmak için gereken dakika sayısını girin</span><span class="sxs-lookup"><span data-stu-id="572e2-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="572e2-123">Senaryoyu çalıştırın</span><span class="sxs-lookup"><span data-stu-id="572e2-123">Run the scenario</span></span>

<span data-ttu-id="572e2-124">Destek temsilcisine verilecek Zip dosyası çıkışını toplayın.</span><span class="sxs-lookup"><span data-stu-id="572e2-124">Collect the Zip file output to be given to the Support agent.</span></span>
