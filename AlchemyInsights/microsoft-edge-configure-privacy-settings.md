---
title: Microsoft Edge gizlilik ayarlarını yapılandırma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678863"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="97c28-102">Microsoft Edge gizlilik ayarlarını yapılandırma</span><span class="sxs-lookup"><span data-stu-id="97c28-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="97c28-103">Varsayılan olarak, Microsoft Edge Windows dışı platformlarda dağıtılmışsa, tanılama verileri ve site bilgileri Microsoft 'a gönderilmez.</span><span class="sxs-lookup"><span data-stu-id="97c28-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="97c28-104">Ancak, Microsoft Edge Windows 10 ' da dağıtılırsa, tanılama verileri ve site bilgileri kullanıcıların [Windows tanılama veri ayarlarına](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)göre gönderilir.</span><span class="sxs-lookup"><span data-stu-id="97c28-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="97c28-105">Microsoft Edge 'in kuruluşunuz için veri toplamayı nasıl işlediğini yapılandırmak için aşağıdaki grup ilkelerini kullanın:</span><span class="sxs-lookup"><span data-stu-id="97c28-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="97c28-106">[Metricsreportingenabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Bu ilke, kullanımı ve çökme ile ilgili verilerin raporlamasını verir.</span><span class="sxs-lookup"><span data-stu-id="97c28-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="97c28-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Bu Ilke, Microsoft hizmetlerini geliştirmek için kullanılan site bilgilerini gönderir.</span><span class="sxs-lookup"><span data-stu-id="97c28-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="97c28-108">Daha fazla bilgi edinmek için [ilke ayarlarını yapılandırma](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="97c28-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>