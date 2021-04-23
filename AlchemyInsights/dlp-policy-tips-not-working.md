---
title: DLP İlkesi İpuçları çalışmıyor
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 68387bf6f5f91657f1d853b9d67bdea6fac21bde
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952212"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="035b6-102">DLP İlkesi İpucu sorunları</span><span class="sxs-lookup"><span data-stu-id="035b6-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="035b6-103">**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="035b6-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="035b6-104">Tam zorlama modunda Güvenlik ve Uyumluluk Merkezi'nde DLP ilkenize & ilke ipuçlarını yapılandırmak için, şunları yapın:</span><span class="sxs-lookup"><span data-stu-id="035b6-104">To configure policy tips on your DLP policy in the Security & Compliance center in full enforcement mode, do the following:</span></span>

- <span data-ttu-id="035b6-105">DLP kuralında ilke **ipuçlarının** etkinleştirildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="035b6-105">Ensure policy tips have been **enabled** on the DLP rule.</span></span> <span data-ttu-id="035b6-106">Adımlar için bkz. [E-posta bildirimleri gönderme ve DLP ilkeleriyle ilgili ilke ipuçlarını gösterme.](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="035b6-106">For steps, see [Send email notifications and show policy tips for DLP policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="035b6-107">İçeriğinizin, Hassas bilgi türü varlık tanımlarında belirtilen kuralı tetiklemesi için [gerekenle eşlendiğinden emin olma.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="035b6-107">Ensure your content matches what is required to trigger the rule outlined in [Sensitive information type entity definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

<span data-ttu-id="035b6-108">İlke ipuçları hem OWA'da hem de Outlook'ta görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="035b6-108">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="035b6-109">Bununla birlikte, Outlook 2013 veya sonraki bir kullanıyorsanız, ilke ipuçları yalnızca belirli koşullarda görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="035b6-109">However, when using Outlook 2013 or later, policy tips are displayed only under certain conditions.</span></span> <span data-ttu-id="035b6-110">Belirli koşullar listesi için, İlke [İpuçları'nın görüntülenmesi için bkz. Outlook 2013 veya sonraki bir yıl için desteklenen koşullar](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="035b6-110">For the specific conditions list, see [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="035b6-111">DLP İlkesi ipuçları hakkında bilgi için bkz. [DLP İlkesi İpuçları Başvurusu ve](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) DLP İlkesi ipuçları için Destek [Matrisi.](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps)</span><span class="sxs-lookup"><span data-stu-id="035b6-111">For information on DLP Policy tips, see [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and [Support Matrix for DLP Policy tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span></span>