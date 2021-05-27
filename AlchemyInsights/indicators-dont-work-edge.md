---
title: Edge tarayıcısı kullanılarak göstergeler çalışmıyor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676576"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="efaec-102">Edge tarayıcısı kullanılarak göstergeler çalışmıyor</span><span class="sxs-lookup"><span data-stu-id="efaec-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="efaec-103">Siz bir Gösterge oluşturduktan sonra, Edge (SmartScreen) tarafından buna gerek yok.</span><span class="sxs-lookup"><span data-stu-id="efaec-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="efaec-104">Daha fazla bilgi için [bkz. IP'ler ve URL'ler/etki alanları için göstergeler oluşturma.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="efaec-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="efaec-105">1. Adım: Aşağıdakilerin</span><span class="sxs-lookup"><span data-stu-id="efaec-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="efaec-106">Göstergenin doğru olduğunu doğrulayın (IP/URL'de yazım hatası yok, doğru eylem, doğru RBAC grupları).</span><span class="sxs-lookup"><span data-stu-id="efaec-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="efaec-107">Olası gecikme sürelerini dikkate almak için göstergeyi oluşturdukten sonra en az 2 saat bekleyin.</span><span class="sxs-lookup"><span data-stu-id="efaec-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="efaec-108">Sistemlerin Uç Nokta için Microsoft Defender'a ekli olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="efaec-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="efaec-109">Sistemlerin Bulut ile iletişim kurayalı olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="efaec-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="efaec-110">Test sitesine gidip SmartScreen'in etkinleştirildiğinden ve erişilebilir olduğunu [doğrulayın.](https://demo.smartscreen.msft.net)</span><span class="sxs-lookup"><span data-stu-id="efaec-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="efaec-111">2. Adım: Olası sorunu giderme</span><span class="sxs-lookup"><span data-stu-id="efaec-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="efaec-112">İstemcinin gereksinimleri karşı olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="efaec-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="efaec-113">Ayrıntılar için [bkz. IP'ler ve URL'ler/etki alanları için göstergeler oluşturma.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="efaec-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="efaec-114">Edge tarayıcısının en son sürümünü çalıştırmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="efaec-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="efaec-115">En son sürümü bulmak için [bkz. Sahip Microsoft Edge sürümüne sahip olun.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="efaec-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="efaec-116">Edge tarayıcısını yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="efaec-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="efaec-117">Ayarda bir gösterge bulunan siteye gidin.</span><span class="sxs-lookup"><span data-stu-id="efaec-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="efaec-118">Site beklendiği gibi görünmüyorsa, 3. Adıma geçin.</span><span class="sxs-lookup"><span data-stu-id="efaec-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="efaec-119">3. Adım: Veri toplama</span><span class="sxs-lookup"><span data-stu-id="efaec-119">Step 3: Collect data</span></span>

- <span data-ttu-id="efaec-120">**MDEClientAnalyzer tanılama** verilerini toplayın.</span><span class="sxs-lookup"><span data-stu-id="efaec-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="efaec-121">Yönergeler için [bkz. Uç Nokta için Microsoft Defender'a makine ekleme ile ilgili sorunlar.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="efaec-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="efaec-122">Fiddler izlemesini yükleme ve toplama konusunda sorun görmüyorsanız bkz. [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="efaec-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="efaec-123">Microsoft Desteği'nin yönlendirmelerini tercih ediyorsanız destek vakalarını açmak için aşağıdaki Destek simgesini seçin.</span><span class="sxs-lookup"><span data-stu-id="efaec-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
