---
title: Office 365 DKIM Kurulumu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666284"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="d0aaf-102">Office 365 DKIM Kurulumu</span><span class="sxs-lookup"><span data-stu-id="d0aaf-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="d0aaf-103">Office 365'te özel etki alanları için yapılandırma DKIM tam talimatları [burada](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="d0aaf-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="d0aaf-104">Özel **her** etki alanı için **iki** DKIM CNAME kayıtlarını etki alanınızın DNS barındırma hizmeti (genellikle, etki alanı Kaydedicisi) oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="d0aaf-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="d0aaf-105">Örneğin, contoso.com ve fourthcoffee.com dört DKIM CNAME kaydı gerektirir: iki contoso.com ve iki fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="d0aaf-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="d0aaf-106">DKIM CNAME kayıtları özel **her** etki alanı için aşağıdaki biçimi kullanın:</span><span class="sxs-lookup"><span data-stu-id="d0aaf-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="d0aaf-107">**Ana bilgisayar adı**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="d0aaf-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="d0aaf-108">**Adresine veya değer noktaları**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="d0aaf-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="d0aaf-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="d0aaf-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="d0aaf-110">**Ana bilgisayar adı**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="d0aaf-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="d0aaf-111">**Adresine veya değer noktaları**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="d0aaf-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="d0aaf-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="d0aaf-112">**TTL**: 3600</span></span>

   <span data-ttu-id="d0aaf-113">\<DomainGUID\> sol tarafındaki metin `.mail.protection.outlook.com` , özelleştirilmiş MX kaydında özel etki alanı (örneğin, `contoso-com` contoso.com etki alanı).</span><span class="sxs-lookup"><span data-stu-id="d0aaf-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="d0aaf-114">\<InitialDomain\> Office 365 (örneğin, contoso.onmicrosoft.com) için kaydolurken kullandığınız etki alanıdır.</span><span class="sxs-lookup"><span data-stu-id="d0aaf-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="d0aaf-115">CNAME kayıtları için özel etki alanlarınızı oluşturduktan sonra aşağıdaki yönergeleri izleyin:</span><span class="sxs-lookup"><span data-stu-id="d0aaf-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="d0aaf-116">bir.</span><span class="sxs-lookup"><span data-stu-id="d0aaf-116">a.</span></span> <span data-ttu-id="d0aaf-117">Sahip olduğunuz iş veya okul hesabı ile [Office 365'te oturum açın](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4).</span><span class="sxs-lookup"><span data-stu-id="d0aaf-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="d0aaf-118">b.</span><span class="sxs-lookup"><span data-stu-id="d0aaf-118">b.</span></span> <span data-ttu-id="d0aaf-119">Sol üst köşedeki uygulama başlatıcı simgesini seçin ve sonra da **Yönetici**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="d0aaf-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="d0aaf-120">c.</span><span class="sxs-lookup"><span data-stu-id="d0aaf-120">c.</span></span> <span data-ttu-id="d0aaf-121">Sol gezinti, **Yönetim** ' i genişletin ve **Exchange**seçin.</span><span class="sxs-lookup"><span data-stu-id="d0aaf-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="d0aaf-122">d.</span><span class="sxs-lookup"><span data-stu-id="d0aaf-122">d.</span></span> <span data-ttu-id="d0aaf-123">**Koruma**Git > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="d0aaf-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="d0aaf-124">e.</span><span class="sxs-lookup"><span data-stu-id="d0aaf-124">e.</span></span> <span data-ttu-id="d0aaf-125">Etki alanını seçin ve sonra **etkinleştirmek** için **oturum DKIM imza ile bu etki alanı için iletileri**seçin.</span><span class="sxs-lookup"><span data-stu-id="d0aaf-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="d0aaf-126">Özel her etki alanı için bu adımı yineleyin.</span><span class="sxs-lookup"><span data-stu-id="d0aaf-126">Repeat this step for each custom domain.</span></span>
