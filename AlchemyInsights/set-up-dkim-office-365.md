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
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645692"
---
# <a name="setup-dkim"></a><span data-ttu-id="95f5f-102">Kurulum DKIM</span><span class="sxs-lookup"><span data-stu-id="95f5f-102">Setup DKIM</span></span>

<span data-ttu-id="95f5f-103">Microsoft 365'teki özel etki alanları için DKIM yapılandırmak için tam yönergeler [burada.](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="95f5f-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="95f5f-104">**Her** özel etki alanı için, etki alanınızın DNS barındırma hizmetinde (genellikle etki alanı kayıt şirketi) **iki** DKIM CNAME kaydı oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="95f5f-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="95f5f-105">Örneğin, contoso.com ve fourthcoffee.com dört DKIM CNAME kaydı gerektirir: ikisi contoso.com için, ikisi fourthcoffee.com için.</span><span class="sxs-lookup"><span data-stu-id="95f5f-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="95f5f-106">**Her** özel etki alanı için DKIM CNAME kayıtları aşağıdaki biçimleri kullanır:</span><span class="sxs-lookup"><span data-stu-id="95f5f-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="95f5f-107">**Ev sahibi adı**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="95f5f-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="95f5f-108">**Adrese veya değere işaret:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="95f5f-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="95f5f-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="95f5f-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="95f5f-110">**Ev sahibi adı**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="95f5f-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="95f5f-111">**Adrese veya değere işaret:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="95f5f-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="95f5f-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="95f5f-112">**TTL**: 3600</span></span>

   <span data-ttu-id="95f5f-113">\<DomainGUID,\> özel etki alanı `.mail.protection.outlook.com` için özelleştirilmiş MX kaydının solundaki `contoso-com` metindir (örneğin, etki alanı contoso.com için).</span><span class="sxs-lookup"><span data-stu-id="95f5f-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="95f5f-114">\<InitialDomain,\> Microsoft 365'e kaydolduğunuzda kullandığınız etki alanıdır (örneğin, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="95f5f-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="95f5f-115">Özel etki alanlarınızın CNAME kayıtlarını oluşturduktan sonra aşağıdaki yönergeleri tamamlayın:</span><span class="sxs-lookup"><span data-stu-id="95f5f-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="95f5f-116">A.</span><span class="sxs-lookup"><span data-stu-id="95f5f-116">a.</span></span> <span data-ttu-id="95f5f-117">iş veya okul hesabınızla [Microsoft 365'te oturum açın.](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)</span><span class="sxs-lookup"><span data-stu-id="95f5f-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="95f5f-118">B.</span><span class="sxs-lookup"><span data-stu-id="95f5f-118">b.</span></span> <span data-ttu-id="95f5f-119">Sol üst köşedeki uygulama başlatıcı simgesini seçin ve ardından **Yönetici**’yi seçin.</span><span class="sxs-lookup"><span data-stu-id="95f5f-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="95f5f-120">C.</span><span class="sxs-lookup"><span data-stu-id="95f5f-120">c.</span></span> <span data-ttu-id="95f5f-121">Sol alt gezintide, **Yönetici'yi** genişletin ve **Exchange'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="95f5f-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="95f5f-122">D.</span><span class="sxs-lookup"><span data-stu-id="95f5f-122">d.</span></span> <span data-ttu-id="95f5f-123">**Koruma** > **DKIM**gidin.</span><span class="sxs-lookup"><span data-stu-id="95f5f-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="95f5f-124">E.</span><span class="sxs-lookup"><span data-stu-id="95f5f-124">e.</span></span> <span data-ttu-id="95f5f-125">Etki alanını seçin ve ardından **DKIM imzaları olan bu etki alanı için Oturum İmza iletilerini** **etkinleştir'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="95f5f-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="95f5f-126">Her özel etki alanı için bu adımı yineleyin.</span><span class="sxs-lookup"><span data-stu-id="95f5f-126">Repeat this step for each custom domain.</span></span>
