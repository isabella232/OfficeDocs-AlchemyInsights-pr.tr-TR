---
title: Microsoft Edge'de gizlilik ayarlarını yapılandırma
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405729"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="0bdab-102">Microsoft Edge'de gizlilik ayarlarını yapılandırma</span><span class="sxs-lookup"><span data-stu-id="0bdab-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="0bdab-103">Varsayılan olarak, Microsoft Edge Windows dışı platformlarda dağıtılırsa, tanılama verileri ve site bilgileri Microsoft'a gönderilmez.</span><span class="sxs-lookup"><span data-stu-id="0bdab-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="0bdab-104">Bununla birlikte, Microsoft Edge Windows 10'da dağıtılırsa, tanılama verileri ve site bilgileri kullanıcıların Windows Tanılama veri [ayarlarına göre gönderilir.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="0bdab-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="0bdab-105">Microsoft Edge'in kurum için veri toplamayı nasıl işley olduğunu yapılandırmak için aşağıdaki grup ilkelerini kullanın:</span><span class="sxs-lookup"><span data-stu-id="0bdab-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="0bdab-106">[MetricsReportingEnabled,](https://go.microsoft.com/fwlink/?linkid=2132470) kullanım ve kilitlenmeyle ilgili verilerin raporlanmasına olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="0bdab-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="0bdab-107">[SendSiteInfoToImproveServices,](https://go.microsoft.com/fwlink/?linkid=2132470) Microsoft hizmetlerini geliştirmek için kullanılan site bilgilerini gönderir.</span><span class="sxs-lookup"><span data-stu-id="0bdab-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="0bdab-108">Daha fazla bilgi edinmek için bkz. [İlke ayarlarını yapılandırma.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="0bdab-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
