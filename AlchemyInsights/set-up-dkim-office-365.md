---
title: Kurulum DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509404"
---
# <a name="setup-dkim"></a><span data-ttu-id="e03a2-102">Kurulum DKIM</span><span class="sxs-lookup"><span data-stu-id="e03a2-102">Setup DKIM</span></span>

<span data-ttu-id="e03a2-103">Microsoft 365'teki özel etki alanları için DKIM yapılandırmak için tam yönergeler [burada.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)</span><span class="sxs-lookup"><span data-stu-id="e03a2-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="e03a2-104">**Her** özel etki alanı için, etki alanınızın DNS barındırma hizmetinde (genellikle etki alanı kayıt şirketi) **iki** DKIM CNAME kaydı oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="e03a2-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="e03a2-105">Örneğin, contoso.com ve fourthcoffee.com dört DKIM CNAME kaydı gerektirir: ikisi contoso.com için, ikisi fourthcoffee.com için.</span><span class="sxs-lookup"><span data-stu-id="e03a2-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="e03a2-106">**Her** özel etki alanı için DKIM CNAME kayıtları aşağıdaki biçimleri kullanır:</span><span class="sxs-lookup"><span data-stu-id="e03a2-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="e03a2-107">**Ev sahibi adı**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="e03a2-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="e03a2-108">**Adrese veya değere işaret:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="e03a2-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="e03a2-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="e03a2-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="e03a2-110">**Ev sahibi adı**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="e03a2-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="e03a2-111">**Adrese veya değere işaret:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="e03a2-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="e03a2-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="e03a2-112">**TTL**: 3600</span></span>

   <span data-ttu-id="e03a2-113">\<DomainGUID\>`.mail.protection.outlook.com`özel etki alanı için özelleştirilmiş MX kaydında solundaki metindir (örneğin, `contoso-com` etki alanı contoso.com).</span><span class="sxs-lookup"><span data-stu-id="e03a2-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="e03a2-114">\<InitialDomain\>Microsoft 365'e kaydolduğunuzda kullandığınız etki alanıdır (örneğin, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="e03a2-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="e03a2-115">Özel etki alanlarınızın CNAME kayıtlarını oluşturduktan sonra aşağıdaki yönergeleri tamamlayın:</span><span class="sxs-lookup"><span data-stu-id="e03a2-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="e03a2-116">a.</span><span class="sxs-lookup"><span data-stu-id="e03a2-116">a.</span></span> <span data-ttu-id="e03a2-117">iş veya okul hesabınızla [Microsoft 365'te oturum açın.](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)</span><span class="sxs-lookup"><span data-stu-id="e03a2-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="e03a2-118">b.</span><span class="sxs-lookup"><span data-stu-id="e03a2-118">b.</span></span> <span data-ttu-id="e03a2-119">Sol üst köşedeki uygulama başlatıcı simgesini seçin ve ardından **Yönetici**’yi seçin.</span><span class="sxs-lookup"><span data-stu-id="e03a2-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="e03a2-120">c.</span><span class="sxs-lookup"><span data-stu-id="e03a2-120">c.</span></span> <span data-ttu-id="e03a2-121">Sol alt gezintide, **Yönetici'yi** genişletin ve **Exchange'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="e03a2-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="e03a2-122">D.</span><span class="sxs-lookup"><span data-stu-id="e03a2-122">d.</span></span> <span data-ttu-id="e03a2-123">Koruma **Protection**  >  **DKIM**gidin.</span><span class="sxs-lookup"><span data-stu-id="e03a2-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="e03a2-124">E.</span><span class="sxs-lookup"><span data-stu-id="e03a2-124">e.</span></span> <span data-ttu-id="e03a2-125">Etki alanını seçin ve ardından **DKIM imzaları olan bu etki alanı için Oturum İmza iletilerini** **etkinleştir'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="e03a2-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="e03a2-126">Her özel etki alanı için bu adımı yineleyin.</span><span class="sxs-lookup"><span data-stu-id="e03a2-126">Repeat this step for each custom domain.</span></span>
