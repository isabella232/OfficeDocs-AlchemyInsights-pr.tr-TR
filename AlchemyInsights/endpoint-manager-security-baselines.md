---
title: EndPoint Manager - Güvenlik temelleri
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440913"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="4336e-102">EndPoint Manager - Güvenlik temelleri</span><span class="sxs-lookup"><span data-stu-id="4336e-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="4336e-103">Güvenlik temelleri, konuyla ilgili güvenlik ekipleri tarafından önerilen güvenlik ayarlarını uygulamaya yardımcı olmak üzere önceden yapılandırılmış Windows ayarı gruplarıdır.</span><span class="sxs-lookup"><span data-stu-id="4336e-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="4336e-104">Bu temel gruplar yalnızca istenen ayarları ve değerleri sunacak şekilde özelleştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="4336e-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="4336e-105">Güvenlik temelleri hakkında daha fazla bilgi için bkz. [Intune’da Windows 10 cihazlarını yapılandırmak için güvenlik temellerini kullanma](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="4336e-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="4336e-106">Şu anda aşağıdaki ürünler için güvenlik temelleri sağlanmıştır:</span><span class="sxs-lookup"><span data-stu-id="4336e-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="4336e-107">Windows MDM Güvenlik ayarları</span><span class="sxs-lookup"><span data-stu-id="4336e-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="4336e-108">Uç nokta için Microsoft Defender Güvenliği</span><span class="sxs-lookup"><span data-stu-id="4336e-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="4336e-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="4336e-109">Microsoft Edge</span></span>

<span data-ttu-id="4336e-110">Bu temellerden her biri düzenli aralıklarla güncelleştirilir ve artımlı sürümlerde kullanıma sunulur.</span><span class="sxs-lookup"><span data-stu-id="4336e-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="4336e-111">Temelin güncel yönergelere uyduğundan emin olmak için her sürüm önce sürümlerin ayarlarına yenilerini ekler veya bazılarını kaldırır.</span><span class="sxs-lookup"><span data-stu-id="4336e-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="4336e-112">Uç Nokta Güvenliği’ndeki Güvenlik temelleri konsolu bir sürümden diğerine yapılan değişiklikleri görünür hale getirerek farklı sürümlerin karşılaştırılmasına olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="4336e-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="4336e-113">Güvenlik temelinin dağıtılacak olan sürümünü en etkili şekilde değiştirme yönergeleri için bkz. [Microsoft Intune’da güvenlik temeli profillerini yönetme](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="4336e-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="4336e-114">Güvenlik temelini dağıttıktan sonra, dağıtımın durumunu izleyebilir ve tek tek cihazlara göre ayarları gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4336e-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="4336e-115">**Not:** Güvenlik temellerine ilişkin raporlama verilerinin görüntülenmesi, bir cihaza ilk dağıtım yapıldıktan sonra 24 saat kadar ve sonraki güncelleştirmelerde 6 saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="4336e-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="4336e-116">Temel ayarının uygulanmamasının en yaygın nedeni, aynı ayarın farklı bir profilde kullanılıyor olmasıdır.</span><span class="sxs-lookup"><span data-stu-id="4336e-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="4336e-117">Belirli bir cihazda bu senaryoyu araştırmak için, Güvenlik Temeli profilinin Cihaz Durumu düğümünden söz konusu cihaz seçilebilir.</span><span class="sxs-lookup"><span data-stu-id="4336e-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="4336e-118">Ayrıntılar için bkz. [Güvenlik temelleri için çakışmaları çözme](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="4336e-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>