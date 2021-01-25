---
title: Uygulama geliştirme sorunları
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974764"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="48dbf-102">Uygulama geliştirme sorunları</span><span class="sxs-lookup"><span data-stu-id="48dbf-102">Issues developing applications</span></span>

<span data-ttu-id="48dbf-103">Azure Active Directory (AD) uygulamalarını oluştururken sık karşılaşılan sorunları gidermek için aşağıdaki makalelere bakın:</span><span class="sxs-lookup"><span data-stu-id="48dbf-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="48dbf-104">Uygulamada yalnızca Chrome tarayıcısını kullanarak oturum açarken sorun yaşıyorum</span><span class="sxs-lookup"><span data-stu-id="48dbf-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="48dbf-105">Uygulamam için belirteç yaşam süresi varsayılanlarını nasıl değiştireceğinizi bilmiyorum</span><span class="sxs-lookup"><span data-stu-id="48dbf-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="48dbf-106">Uygulama izninin nasıl çalıştığı hakkında konuşdum</span><span class="sxs-lookup"><span data-stu-id="48dbf-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="48dbf-107">Uygulamama izin vermeyi bilmiyorum</span><span class="sxs-lookup"><span data-stu-id="48dbf-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="48dbf-108">Temsilci ile uygulama izinleri arasındaki farkı anlayamıyorum</span><span class="sxs-lookup"><span data-stu-id="48dbf-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="48dbf-109">\***Azure Active Directory kimlik doğrulama kütüphanesi (ADAL) ve Azure AD GRAFIĞI API (AAD Graph) _ desteği sonu**</span><span class="sxs-lookup"><span data-stu-id="48dbf-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="48dbf-110">30 Haziran 2020 ' de başlıyor, artık Azure Active Directory kimlik doğrulama kitaplığı (ADAL) ve Azure AD grafiği API (AAD Graph) için yeni özellikler ekleyemeyecektir.</span><span class="sxs-lookup"><span data-stu-id="48dbf-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="48dbf-111">Teknik destek ve güvenlik güncelleştirmelerini sağlamaya devam edeceğiz ancak artık özellik güncelleştirmeleri sağlamaz.</span><span class="sxs-lookup"><span data-stu-id="48dbf-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="48dbf-112">30 Haziran 2022 ' de başlıyor, ADAL ve AAD Graph için desteği sona eririz ve artık teknik destek veya güvenlik güncelleştirmeleri sağlamaz.</span><span class="sxs-lookup"><span data-stu-id="48dbf-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="48dbf-113">Bu koşulun sonucu olarak aşağıdaki etkiler:</span><span class="sxs-lookup"><span data-stu-id="48dbf-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="48dbf-114">Mevcut işletim sistemi sürümlerinde ADAL kullanan uygulamalar, bu saatten sonra çalışmaya devam edecektir, ancak teknik destek veya güvenlik güncelleştirmelerini alamaz.</span><span class="sxs-lookup"><span data-stu-id="48dbf-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="48dbf-115">Bu saatten sonra AAD grafiği kullanan uygulamalar artık AAD grafik uç noktasından yanıt alamıyor</span><span class="sxs-lookup"><span data-stu-id="48dbf-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="48dbf-116">_ *Adal geçişi*\*</span><span class="sxs-lookup"><span data-stu-id="48dbf-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="48dbf-117">Microsoft uygulamalarını kullanıyorsanız, en son özellikleri ve güvenlik güncelleştirmelerini içeren Microsoft kimlik doğrulama kitaplığı (MSAL) güncelleştirmesini öneririz.</span><span class="sxs-lookup"><span data-stu-id="48dbf-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="48dbf-118">Bu öneri, Microsoft 'un uygulamalarını MSAL-of support son tarihine kadar uygulamalarını başlatma işlemini başlatıyor.</span><span class="sxs-lookup"><span data-stu-id="48dbf-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="48dbf-119">Microsoft 'un uygulamalarını MSAL 'a geçirmek, uygulamaların MSAL 'un devam eden güvenlik ve özellik geliştirmelerinin avantajlarından yararlanmasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="48dbf-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="48dbf-120">ADAL SSS 'sini okuyun</span><span class="sxs-lookup"><span data-stu-id="48dbf-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="48dbf-121">Uygulamaları platforma göre nasıl geçirebileceğiniz hakkında bilgi edinin</span><span class="sxs-lookup"><span data-stu-id="48dbf-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="48dbf-122">Hangi uygulamalarınızı ADAL kullanarak kullanacağınızı anlamayla ilgili yardıma ihtiyacınız varsa, tüm uygulamalarınızın kaynak kodunu gözden geçirmenizi ve varsa tüm bağımsız yazılım satıcılarına (ISV 'Ler) veya uygulama sağlayıcılarını gözden geçirmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="48dbf-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="48dbf-123">Microsoft desteği size kiracınızdaki Microsoft olmayan tüm ADAL uygulamalarının bir listesini sağlayabilir.</span><span class="sxs-lookup"><span data-stu-id="48dbf-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="48dbf-124">**AAD grafik geçişi**</span><span class="sxs-lookup"><span data-stu-id="48dbf-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="48dbf-125">AAD Graph kullanan uygulamalar için, AAD grafik uygulamalarını Microsoft Graph 'a geçirmek için kılavuzumuzu izleyin:</span><span class="sxs-lookup"><span data-stu-id="48dbf-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="48dbf-126">[Geçiş denetim listesi başlangıç noktası sağlar](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="48dbf-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="48dbf-127">Azure App Registration Portal 'da, AAD grafiğini kullanan uygulamalar gösterilir.</span><span class="sxs-lookup"><span data-stu-id="48dbf-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="48dbf-128">Tüm uygulamalarınızın kaynak kodunu incelemenizi öneririz ve uygulanabiliyorsa, herhangi bir bağımsız yazılım satıcısı (ISV) veya uygulama sağlayıcılarını kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="48dbf-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="48dbf-129">Microsoft destek, kiracınızdaki AAD grafik kullanımıyla ilgili bilgileri de sağlayabilir.</span><span class="sxs-lookup"><span data-stu-id="48dbf-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







