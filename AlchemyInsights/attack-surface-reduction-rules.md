---
title: Saldırı yüzeyini azaltma kuralları
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
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676570"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="d8dcc-102">Saldırı yüzeyini azaltma kuralları</span><span class="sxs-lookup"><span data-stu-id="d8dcc-102">Attack surface reduction rules</span></span>

<span data-ttu-id="d8dcc-103">Dosya veya klasörlerin dışlamaları saldırı yüzeyini azaltma kuralları tarafından sağlanan korumayı ciddi ölçüde azaltır.</span><span class="sxs-lookup"><span data-stu-id="d8dcc-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="d8dcc-104">Kural tarafından engellenmiş olan dosyaların çalışmasına izin verilir ve hiçbir rapor veya olay kaydedilmiyor.</span><span class="sxs-lookup"><span data-stu-id="d8dcc-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="d8dcc-105">Dışlama, dışlamalara izin olan tüm kurallara uygulanır.</span><span class="sxs-lookup"><span data-stu-id="d8dcc-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="d8dcc-106">ASR dışlamaları, dışlamalarda olduğu gibi Microsoft Defender Virüsten Koruma kullanır.</span><span class="sxs-lookup"><span data-stu-id="d8dcc-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="d8dcc-107">Ayrıntılar için bkz. [Taramalarda dışlamaları yapılandırma Microsoft Defender Virüsten Koruma doğrulama.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="d8dcc-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="d8dcc-108">Sorunlardan kaçınmak için, [dışlamaları tanımlarken kaçınılması gereken yaygın hataları gözden geçirin.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="d8dcc-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="d8dcc-109">Tüm ASR kuralları dışlamaları desteklemez.</span><span class="sxs-lookup"><span data-stu-id="d8dcc-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="d8dcc-110">Kuralınız dışlamaları destekleyip desteklemedi bunu doğrulamak için Saldırı yüzeyini azaltma [kuralları tablosuna bakın.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="d8dcc-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="d8dcc-111">Saldırı yüzeyini azaltma kuralları</span><span class="sxs-lookup"><span data-stu-id="d8dcc-111">Attack surface reduction rules</span></span>

<span data-ttu-id="d8dcc-112">Organizasyon saldırı yüzeyiniz, bir saldırganın kuruluş cihazlarını veya ağlarını tehlikeye atabilmesi için güvenlik ödünleri olan tüm yerleri içerir.</span><span class="sxs-lookup"><span data-stu-id="d8dcc-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="d8dcc-113">Saldırı yüzeyinizi azaltmak, kuruluş cihazlarını ve ağın korunması anlamına gelir; bu da saldırı gerçekleştirmek için daha az yol bırakır.</span><span class="sxs-lookup"><span data-stu-id="d8dcc-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="d8dcc-114">Uç nokta için Microsoft Defender'da saldırı yüzeyini azaltma kurallarını yapılandırmanıza yardımcı olabilir.</span><span class="sxs-lookup"><span data-stu-id="d8dcc-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="d8dcc-115">Daha fazla bilgi için bkz.:</span><span class="sxs-lookup"><span data-stu-id="d8dcc-115">For more information, see:</span></span>

- [<span data-ttu-id="d8dcc-116">ASR kuralı GUID'lerini adla eşleme</span><span class="sxs-lookup"><span data-stu-id="d8dcc-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="d8dcc-117">ASR kuralları gereksinimleri:</span><span class="sxs-lookup"><span data-stu-id="d8dcc-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="d8dcc-118">Windows 10 Pro, sürüm 1709 veya sonrası</span><span class="sxs-lookup"><span data-stu-id="d8dcc-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="d8dcc-119">Windows 10 Enterprise, sürüm 1709 veya sonrası</span><span class="sxs-lookup"><span data-stu-id="d8dcc-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="d8dcc-120">Windows Sunucu, sürüm 1803 (Yarı Yıllık Kanal) veya sonraki sürümler</span><span class="sxs-lookup"><span data-stu-id="d8dcc-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="d8dcc-121">Uygulanacak doğru dışlamayı belirleme</span><span class="sxs-lookup"><span data-stu-id="d8dcc-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="d8dcc-122">Microsoft-Windows-Windows Defender/Operational günlüğünde eventID 1121 veya 1122'i bakın.</span><span class="sxs-lookup"><span data-stu-id="d8dcc-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="d8dcc-123">Engelleme senaryosunu ve bağlamı değerlendirin ve bu senaryonun engellemesini kaldırmanız gerektiğini onaylayın.</span><span class="sxs-lookup"><span data-stu-id="d8dcc-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="d8dcc-124">Olay ayrıntılarında Yol değerini okuyun; bu, dışlamayı tanımlayan değerdir.</span><span class="sxs-lookup"><span data-stu-id="d8dcc-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="d8dcc-125">Dışlama mümkün olduğunca katı hale geldi.</span><span class="sxs-lookup"><span data-stu-id="d8dcc-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="d8dcc-126">Gerektiğinde bir joker karakter uygulayabilirsiniz (örneğin, Kullanıcı değişkeninin yerini değiştirin).</span><span class="sxs-lookup"><span data-stu-id="d8dcc-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="d8dcc-127">Dışlamayı dağıtım ihtiyaçlarına göre uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d8dcc-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="d8dcc-128">Ayrıntılı bilgi için Saldırı [yüzeyini azaltma kurallarını özelleştirme .](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)</span><span class="sxs-lookup"><span data-stu-id="d8dcc-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="d8dcc-129">Dışlamalara devam etmek mümkün değil</span><span class="sxs-lookup"><span data-stu-id="d8dcc-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="d8dcc-130">Kuralın dışlamalarını destekle ilgili olup olmadığını belirler.</span><span class="sxs-lookup"><span data-stu-id="d8dcc-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="d8dcc-131">Ayrıntılı bilgi için Saldırı [yüzeyini azaltma kuralları 'ne bakın.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="d8dcc-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="d8dcc-132">Uygulanan dışlamaları gözden geçirme ve yazım hataları veya yanlış yapılan joker karakterlerle ilgili olay verileriyle doğrulama.</span><span class="sxs-lookup"><span data-stu-id="d8dcc-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="d8dcc-133">Daha fazla bilgi için [bkz. Desteklenen dışlama türleri](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="d8dcc-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="d8dcc-134">kuralın etkisi çok yüksekse, daha fazla doğrulama gerçekleştirmek için kuralı (geri) Denetim moduna taşımayı göz önünde bulundurabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d8dcc-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="d8dcc-135">Ayrıntılar için bkz. [Uç nokta özellikleri için Microsoft Defender'ın denetim modunda nasıl çalışacı olduğunu test edin.](/microsoft-365/security/defender-endpoint/audit-windows-defender)</span><span class="sxs-lookup"><span data-stu-id="d8dcc-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="d8dcc-136">Bu komutu kullanarak destek olaylarını açmak için destek verilerini toplayın:</span><span class="sxs-lookup"><span data-stu-id="d8dcc-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="d8dcc-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="d8dcc-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="d8dcc-138">Daha fazla bilgi için [bkz. Uç Noktalar için Microsoft Defender'a makine ekleme ile ilgili sorunlar.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="d8dcc-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
