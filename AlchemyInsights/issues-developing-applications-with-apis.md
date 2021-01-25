---
title: API ile uygulama geliştirme sorunları
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975021"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="50e6f-102">API ile uygulama geliştirme sorunları</span><span class="sxs-lookup"><span data-stu-id="50e6f-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="50e6f-103">Azure Active Directory Graph API 'sini kullanmaya başlamak için, [Azure AD GRAFIĞI API hızlı başlangıç kılavuzuna](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) bakın veya [etkileşimli Azure AD grafiği API başvuru belgelerine](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)bakın.</span><span class="sxs-lookup"><span data-stu-id="50e6f-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="50e6f-104">**Azure Active Directory kimlik doğrulama kütüphanesi (ADAL) ve Azure AD grafiği API (AAD grafiği) için destek sonu**</span><span class="sxs-lookup"><span data-stu-id="50e6f-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="50e6f-105">**30 haziran 2020**' de başlıyor, artık adal ve Azure AD grafiğinin yeni özelliklerini eklemeiyoruz.</span><span class="sxs-lookup"><span data-stu-id="50e6f-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="50e6f-106">Teknik destek ve güvenlik güncelleştirmelerini sağlamaya devam edeceğiz ancak artık özellik güncelleştirmeleri sağlamaz.</span><span class="sxs-lookup"><span data-stu-id="50e6f-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="50e6f-107">**30 haziran 2022**' de BAŞLıYOR, adal ve Azure AD Graph için desteği son verecek ve artık teknik destek veya güvenlik güncelleştirmeleri sağlayamayacak.</span><span class="sxs-lookup"><span data-stu-id="50e6f-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="50e6f-108">Mevcut işletim sistemi sürümlerinde ADAL kullanan uygulamalar, bu saatten sonra çalışmaya devam edecektir, ancak teknik destek veya güvenlik güncelleştirmelerini alamaz.</span><span class="sxs-lookup"><span data-stu-id="50e6f-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="50e6f-109">Bu saatten sonra Azure AD grafiği kullanan uygulamalar artık Azure AD grafiği uç noktasından yanıt alamaz.</span><span class="sxs-lookup"><span data-stu-id="50e6f-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="50e6f-110">**ADAL geçişi**</span><span class="sxs-lookup"><span data-stu-id="50e6f-110">**ADAL Migration**</span></span>

<span data-ttu-id="50e6f-111">En son özellikleri ve güvenlik güncelleştirmelerini içeren [Microsoft kimlik doğrulama kitaplığı (msal)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)güncelleştirmesini öneririz.</span><span class="sxs-lookup"><span data-stu-id="50e6f-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="50e6f-112">Microsoft uygulamalarını kullanıyorsanız, Microsoft 'un uygulamalarını MSAL 'in destek zamanı son tarihine geçirmeyle MSAL devam eden güvenlik ve özellik geliştirmelerinin avantajlarından yararlanabileceği konusunda unutmayın.</span><span class="sxs-lookup"><span data-stu-id="50e6f-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="50e6f-113">[Adal SSS 'Sini okuyun](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="50e6f-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="50e6f-114">[Uygulamaları tek tek platforma geçirme hakkında bilgi edinin](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="50e6f-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="50e6f-115">Hangi uygulamalarınızı ADAL kullanarak anladığınızdan yardım gerekirse, tüm uygulamalarınızın kaynak kodunu gözden geçirmenizi ve uygulanabiliyorsa, herhangi bir ISV veya uygulama sağlayıcısına ulaşın.</span><span class="sxs-lookup"><span data-stu-id="50e6f-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="50e6f-116">Microsoft desteği size kiracınızdaki Microsoft olmayan tüm ADAL uygulamalarının bir listesini sağlayabilir.</span><span class="sxs-lookup"><span data-stu-id="50e6f-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="50e6f-117">**AAD grafik geçişi**</span><span class="sxs-lookup"><span data-stu-id="50e6f-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="50e6f-118">Azure AD grafiği kullanan uygulamalar için, [Azure AD grafiği uygulamalarını Microsoft Graph 'a](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)geçirmek için kılavuzumuzu izleyin.</span><span class="sxs-lookup"><span data-stu-id="50e6f-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="50e6f-119">[Geçiş denetim listesi başlangıç noktası sağlar](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="50e6f-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="50e6f-120">Azure App Registration Portal 'da, AAD grafiğini kullanan uygulamalar gösterilir.</span><span class="sxs-lookup"><span data-stu-id="50e6f-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="50e6f-121">Tüm uygulamalarınızın kaynak kodunu incelemenizi öneririz ve uygulanabiliyorsa, herhangi bir ISV veya uygulama sağlayıcısına ulaşın.</span><span class="sxs-lookup"><span data-stu-id="50e6f-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="50e6f-122">Microsoft desteği size kiracınızdaki tüm AAD grafik kullanımının listesini de verebilir.</span><span class="sxs-lookup"><span data-stu-id="50e6f-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="50e6f-123">Uygulamanızın Microsoft Graph 'ta verilere erişmesi için, Kullanıcı veya yöneticinin onay süreci aracılığıyla doğru izinleri vermesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="50e6f-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="50e6f-124">[Microsoft Graph Permissions başvurusu](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) , her bir Microsoft Graph API kümesiyle ilişkili izinleri listeler.</span><span class="sxs-lookup"><span data-stu-id="50e6f-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="50e6f-125">İzinlerin nasıl kullanılacağı hakkında rehberlik de sağlar.</span><span class="sxs-lookup"><span data-stu-id="50e6f-125">It also provides guidance about how to use the permissions.</span></span>
