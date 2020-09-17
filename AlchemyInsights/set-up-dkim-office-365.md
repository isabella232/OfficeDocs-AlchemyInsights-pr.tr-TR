---
title: Kuruluş kurulumu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808727"
---
# <a name="setup-dkim"></a><span data-ttu-id="b31d9-102">Kuruluş kurulumu</span><span class="sxs-lookup"><span data-stu-id="b31d9-102">Setup DKIM</span></span>

<span data-ttu-id="b31d9-103">Microsoft 365 'de özel etki alanları için VSEÇKIM yapılandırması ile ilgili eksiksiz yönergeler [.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)</span><span class="sxs-lookup"><span data-stu-id="b31d9-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="b31d9-104">**Her** özel etki alanı için, etkı alanınızın DNS **two** barındırma hizmetinde (genellikle etki alanı kayıt</span><span class="sxs-lookup"><span data-stu-id="b31d9-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="b31d9-105">Örneğin, contoso.com ve fourthcoffee.com için dört DKIM CNAME kaydı gerekir: contoso.com için iki ve fourthcoffee.com için iki.</span><span class="sxs-lookup"><span data-stu-id="b31d9-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="b31d9-106">**Tüm** özel etki alanları için VSEÇKIM CNAME kayıtları aşağıdaki biçimleri kullanır:</span><span class="sxs-lookup"><span data-stu-id="b31d9-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="b31d9-107">**Ana bilgisayar adı**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="b31d9-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="b31d9-108">**Adres veya değer noktaları**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="b31d9-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="b31d9-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="b31d9-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="b31d9-110">**Ana bilgisayar adı**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="b31d9-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="b31d9-111">**Adres veya değer noktaları**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="b31d9-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="b31d9-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="b31d9-112">**TTL**: 3600</span></span>

   <span data-ttu-id="b31d9-113">\<DomainGUID\>`.mail.protection.outlook.com`özel etki alanı için ÖZELLEŞTIRILMIŞ MX kaydının solundaki metindir (örneğin, `contoso-com` contoso.com).</span><span class="sxs-lookup"><span data-stu-id="b31d9-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="b31d9-114">\<InitialDomain\> , Microsoft 365 (örneğin, contoso.onmicrosoft.com) için kaydolduğunuzda kullandığınız etki alanıdır.</span><span class="sxs-lookup"><span data-stu-id="b31d9-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="b31d9-115">Özel etki alanlarınız için CNAME kayıtlarını oluşturduktan sonra aşağıdaki yönergeleri tamamlayın:</span><span class="sxs-lookup"><span data-stu-id="b31d9-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="b31d9-116">a.</span><span class="sxs-lookup"><span data-stu-id="b31d9-116">a.</span></span> <span data-ttu-id="b31d9-117">iş veya okul hesabınızla [Microsoft 365 oturumu açın](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) .</span><span class="sxs-lookup"><span data-stu-id="b31d9-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="b31d9-118">b.</span><span class="sxs-lookup"><span data-stu-id="b31d9-118">b.</span></span> <span data-ttu-id="b31d9-119">Sol üst köşedeki uygulama başlatıcı simgesini seçin ve ardından **Yönetici**’yi seçin.</span><span class="sxs-lookup"><span data-stu-id="b31d9-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="b31d9-120">c.</span><span class="sxs-lookup"><span data-stu-id="b31d9-120">c.</span></span> <span data-ttu-id="b31d9-121">Sol alt gezintide **yönetici** 'Yi genişletip **Exchange**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="b31d9-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="b31d9-122">d.</span><span class="sxs-lookup"><span data-stu-id="b31d9-122">d.</span></span> <span data-ttu-id="b31d9-123">**Protection**'a gidin  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="b31d9-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="b31d9-124">e.</span><span class="sxs-lookup"><span data-stu-id="b31d9-124">e.</span></span> <span data-ttu-id="b31d9-125">Etki alanını seçin ve ardından **cıkim imzaları ile bu etki alanı Için imza Iletilerini** **Etkinleştir** 'i seçin.</span><span class="sxs-lookup"><span data-stu-id="b31d9-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="b31d9-126">Her özel etki alanı için bu adımı uygulayın.</span><span class="sxs-lookup"><span data-stu-id="b31d9-126">Repeat this step for each custom domain.</span></span>
