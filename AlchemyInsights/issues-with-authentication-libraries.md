---
title: Kimlik Doğrulama Kitaplıkları ile ilgili sorunlar
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063702"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="227ed-102">Kimlik Doğrulama Kitaplıkları ile ilgili sorunlar</span><span class="sxs-lookup"><span data-stu-id="227ed-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="227ed-103">[Microsoft kimlik platformu kimlik doğrulama kitaplıkları,](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) Microsoft tarafından desteklenen ve uyumlu istemci ve orta yazılım kitaplıklarını listeler.</span><span class="sxs-lookup"><span data-stu-id="227ed-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="227ed-104">Microsoft Kimlik Doğrulama Kitaplığı (MSAL), farklı uygulama [senaryolarında kullanmak](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) üzere çeşitli kimlik doğrulama akışlarını destekler.</span><span class="sxs-lookup"><span data-stu-id="227ed-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="227ed-105">Belirteçlerin kimliğini doğrulamak ve almak için, kodundaki yeni bir genel veya gizli istemci uygulamasını başlatmış olursunuz.</span><span class="sxs-lookup"><span data-stu-id="227ed-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="227ed-106">Microsoft Kimlik Doğrulama Kitaplığı'nın (MSAL) istemci uygulamasını başlatılırken çeşitli yapılandırma seçenekleri ayarekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="227ed-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="227ed-107">Daha fazla bilgi edinmek için [bkz. Uygulama yapılandırma seçenekleri.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)</span><span class="sxs-lookup"><span data-stu-id="227ed-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="227ed-108">**Azure Active Directory Kimlik Doğrulama Kitaplığı (ADAL) ve Azure AD Graph API'si (AAD Graph) için destek sonu**</span><span class="sxs-lookup"><span data-stu-id="227ed-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="227ed-109">**30 Haziran 2020'den** itibaren artık ADAL ve Azure AD Graph'e yeni özellikler eklemeyecek.</span><span class="sxs-lookup"><span data-stu-id="227ed-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="227ed-110">Teknik destek ve güvenlik güncellemeleri sağlamaya devam edeceğiz, ancak artık özellik güncellemeleri sunmayacağız.</span><span class="sxs-lookup"><span data-stu-id="227ed-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="227ed-111">**30 Haziran 2022'den** başlayarak, ADAL ve Azure AD Graph desteğini sona erecek ve artık teknik destek veya güvenlik güncelleştirmeleri sağmayacak.</span><span class="sxs-lookup"><span data-stu-id="227ed-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="227ed-112">Mevcut işletim sistemi sürümlerinde ADAL kullanan uygulamalar bu sürenin ardından çalışmaya devam edecektir, ancak teknik destek *veya güvenlik güncelleştirmelerini almayacaktır.*</span><span class="sxs-lookup"><span data-stu-id="227ed-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="227ed-113">Bu sürenin ardından Azure AD Graph kullanan uygulamalar artık Azure AD Graph uç noktasının yanıtlarını almayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="227ed-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="227ed-114">**ADAL Geçişi**</span><span class="sxs-lookup"><span data-stu-id="227ed-114">**ADAL Migration**</span></span>

<span data-ttu-id="227ed-115">En son özelliklere ve güvenlik güncellemelerine sahip olan [Microsoft Kimlik Doğrulama Kitaplığı'na (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) güncelleme yapmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="227ed-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="227ed-116">Microsoft uygulamalarını kullanıyorsanız, Microsoft'un son destek bitiş tarihine kadar uygulamalarını MSAL'a geçmektedir ve MSAL'ın devam eden güvenlik ve özellik geliştirmelerinden yararlanacaklarından da temin edin.</span><span class="sxs-lookup"><span data-stu-id="227ed-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="227ed-117">Daha fazla bilgi için bkz.:</span><span class="sxs-lookup"><span data-stu-id="227ed-117">For more information, see:</span></span>

1. [<span data-ttu-id="227ed-118">ADAL SSS bölümünü okuyunuz</span><span class="sxs-lookup"><span data-stu-id="227ed-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="227ed-119">Uygulamaları platforma göre nasıl taşıyacağınız hakkında bilgi edinin</span><span class="sxs-lookup"><span data-stu-id="227ed-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="227ed-120">Uygulamalardan hangilerinin ADAL'ı kullanabileceğini anlamanız için yardıma ihtiyacınız varsa tüm uygulamalarınızı kaynak kodunu gözden geçirmenizi ve varsa tüm ISV'lere veya uygulama sağlayıcılarına ulaşmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="227ed-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="227ed-121">Microsoft desteği ayrıca kiracınızdaki Microsoft dışı tüm ADAL uygulamalarının bir listesini de sağlayabilir.</span><span class="sxs-lookup"><span data-stu-id="227ed-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="227ed-122">**AAD Graph Geçişi**</span><span class="sxs-lookup"><span data-stu-id="227ed-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="227ed-123">Azure AD Graph kullanan uygulamalar için, Azure AD Graph uygulamalarını Microsoft Graph'e geçirme [yönergelerimizi izleyin.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="227ed-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="227ed-124">Geçiş denetim listemiz bir başlama noktası sağlar.</span><span class="sxs-lookup"><span data-stu-id="227ed-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="227ed-125">Azure uygulama kayıt portalınız, hangi uygulamaların AAD Graph kullandığını gösterir.</span><span class="sxs-lookup"><span data-stu-id="227ed-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="227ed-126">Tüm uygulamalarınızın kaynak kodunu gözden geçirmenizi ve uygunsa, herhangi bir ISV veya uygulama sağlayıcıya ulaşmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="227ed-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="227ed-127">Microsoft desteği, kiracınız için tüm AAD Graph kullanımının bir listesini de sağlar.</span><span class="sxs-lookup"><span data-stu-id="227ed-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="227ed-128">Uygulamanın Microsoft Graph'te verilere erişmesi için, kullanıcı veya yöneticinin izin süreci aracılığıyla ona doğru izinleri ataması gerekir.</span><span class="sxs-lookup"><span data-stu-id="227ed-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="227ed-129">[Microsoft Graph izinleri başvurusu,](https://docs.microsoft.com/graph/permissions-reference) her bir önemli Microsoft Graph API'leri kümesiyle ilişkilendirilmiş izinleri listeler.</span><span class="sxs-lookup"><span data-stu-id="227ed-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="227ed-130">Ayrıca, izinleri kullanma konusunda da yol göstermeyi sağlar.</span><span class="sxs-lookup"><span data-stu-id="227ed-130">It also provides guidance about how to use the permissions.</span></span>
