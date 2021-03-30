---
title: EndPoint Manager - Güvenlik taban çizgisi
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
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421218"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="1ef80-102">EndPoint Manager - Güvenlik taban çizgisi</span><span class="sxs-lookup"><span data-stu-id="1ef80-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="1ef80-103">Güvenlik taban çizgisi, ilgili güvenlik ekipleri tarafından önerilen güvenlik ayarlarını uygulamanıza yardımcı olan önceden yapılandırılmış Windows ayarları gruplarıdır.</span><span class="sxs-lookup"><span data-stu-id="1ef80-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="1ef80-104">Bu taban çizgisi, yalnızca istediğiniz ayarları ve değerleri sunmak için özelleştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="1ef80-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="1ef80-105">Güvenlik taban çizgisi hakkında daha fazla bilgi için Bkz. [Intune'da Windows 10](https://docs.microsoft.com/mem/intune/protect/security-baselines)cihazlarını yapılandırmak için güvenlik taban çizgilerini kullanma.</span><span class="sxs-lookup"><span data-stu-id="1ef80-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="1ef80-106">Şu anda bu ürünlerin taban çizgilerini vardır:</span><span class="sxs-lookup"><span data-stu-id="1ef80-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="1ef80-107">Windows MDM Güvenlik ayarları</span><span class="sxs-lookup"><span data-stu-id="1ef80-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="1ef80-108">EndPoint Güvenliği için Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="1ef80-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="1ef80-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="1ef80-109">Microsoft Edge</span></span>

<span data-ttu-id="1ef80-110">Taban çizgilerinin her biri düzenli olarak güncelleştirilir ve artımlı sürümlerde yayımlanır.</span><span class="sxs-lookup"><span data-stu-id="1ef80-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="1ef80-111">Taban çizgisinin geçerli kılavuz çizgiye uygun olduğundan emin olmak için, her sürüm önceki sürümden ayarları ekler ve kaldırır.</span><span class="sxs-lookup"><span data-stu-id="1ef80-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="1ef80-112">Uç Nokta Güvenliği'nin Güvenlik taban çizgisi konsolu, sürümden sürüme yapılan değişikliklerin görünür olmasıyla farklı sürümlerin karşılaştırmasına olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="1ef80-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="1ef80-113">Temelin hangi sürümünün dağıtılacağı konusunda yol gösterici bilgi için, Microsoft Intune'da güvenlik temeli [profillerini yönetme makalelerine bakın.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)</span><span class="sxs-lookup"><span data-stu-id="1ef80-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="1ef80-114">Güvenlik temelini dağıttırdikten sonra, dağıtım durumunu izleyebilir ve ayarları cihaz temelinde gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1ef80-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="1ef80-115">**Not:** Taban çizgilerinin raporlama verileri, ilk dağıtımdan bir cihaza 24 saat ve daha sonraki güncelleştirmeler için 6 saate kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="1ef80-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="1ef80-116">Taban çizgisi ayarının uygulamamalarının en yaygın nedeni, aynı ayarın farklı bir profilde kullanılıyor olmasıdır.</span><span class="sxs-lookup"><span data-stu-id="1ef80-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="1ef80-117">Bu senaryo, Belirli bir cihaz için, Güvenlik Temeli profilinin Cihaz Durumu düğümünden seçerek araştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1ef80-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="1ef80-118">Ayrıntılar için [bkz. Güvenlik taban çizgilerine ilişkin çakışmaları çözme.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="1ef80-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>