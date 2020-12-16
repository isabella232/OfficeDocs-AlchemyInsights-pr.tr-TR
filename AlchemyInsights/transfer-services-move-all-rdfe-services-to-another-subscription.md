---
title: Aktarma hizmetleri-tüm RDFE hizmetlerini başka bir aboneliğe taşıma
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692180"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="888f9-102">Aktarma hizmetleri-tüm RDFE hizmetlerini başka bir aboneliğe taşıma</span><span class="sxs-lookup"><span data-stu-id="888f9-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="888f9-103">**Kaynakları taşıma**</span><span class="sxs-lookup"><span data-stu-id="888f9-103">**Move resources**</span></span>

<span data-ttu-id="888f9-104">Azure kaynakları, Azure portalı, Azure PowerShell, Azure CLı veya REST API 'yi kullanan aynı aboneliğin altındaki başka bir Azure aboneliğine veya kaynak grubuna geçebilir.</span><span class="sxs-lookup"><span data-stu-id="888f9-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="888f9-105">Kaynakları taşıyabilmek için önce bkz:</span><span class="sxs-lookup"><span data-stu-id="888f9-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="888f9-106">Kaynakları taşımadan önce denetim listesi</span><span class="sxs-lookup"><span data-stu-id="888f9-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="888f9-107">Taşınamayan hizmetler</span><span class="sxs-lookup"><span data-stu-id="888f9-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="888f9-108">Taşıma nasıl doğrulanır</span><span class="sxs-lookup"><span data-stu-id="888f9-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="888f9-109">Hizmetler için kılavuzu taşıma</span><span class="sxs-lookup"><span data-stu-id="888f9-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="888f9-110">Var olan kaynakları başka bir kaynak grubuna veya aboneliğe taşımak için şunları kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="888f9-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="888f9-111">Azure portalı</span><span class="sxs-lookup"><span data-stu-id="888f9-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="888f9-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="888f9-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="888f9-113">Azure CLı</span><span class="sxs-lookup"><span data-stu-id="888f9-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="888f9-114">REST APı 'SI</span><span class="sxs-lookup"><span data-stu-id="888f9-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="888f9-115">Öğretici: [Azure kaynaklarını başka bir kaynak grubuna veya aboneliğe taşıma](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="888f9-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="888f9-116">**Azure Resource Manager ile ilgili sorunları giderme**</span><span class="sxs-lookup"><span data-stu-id="888f9-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="888f9-117">Bazı yaygın Azure dağıtım hatalarını öğrenmek ve bunları çözmek için bilgi almak için aşağıdaki makalelere bakın.</span><span class="sxs-lookup"><span data-stu-id="888f9-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="888f9-118">Dağıtım hatasının hata kodunu bulamazsanız, [hata kodu bul](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)'a bakın.</span><span class="sxs-lookup"><span data-stu-id="888f9-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="888f9-119">Dağıtım hatalarını giderme</span><span class="sxs-lookup"><span data-stu-id="888f9-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="888f9-120">Azure kaynaklarını yeni kaynak grubuna veya aboneliğe taşıma sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="888f9-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="888f9-121">Azure aboneliğinizi ücretsiz olarak öde-to-to-to-to-to-to-to-to-to-to-to-to-to-to-to-to-to-</span><span class="sxs-lookup"><span data-stu-id="888f9-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="888f9-122">Ücretsiz deneme sürümünü güncelleştirmek için, [ücretsiz deneme sürenizi yükseltme veya Microsoft 'un size devam eden ödeme Için Azure aboneliğini yükseltme](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="888f9-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="888f9-123">Bir Kullandıkça Öde hesabını değiştirmek için, bkz: [Azure öde-to](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)-to-to-to-to-to-to-to-to-to</span><span class="sxs-lookup"><span data-stu-id="888f9-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="888f9-124">**Azure Active Directory kiracınıza bir Azure aboneliği eklemek veya ilişkilendirmek için:**</span><span class="sxs-lookup"><span data-stu-id="888f9-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="888f9-125">Oturum açın ve [Azure portalında abonelikler sayfasından](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)kullanmak istediğiniz aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="888f9-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="888f9-126">**Dizini Değiştir**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="888f9-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="888f9-127">Görüntülenen tüm uyarıları gözden geçirin ve ardından **Değiştir**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="888f9-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="888f9-128">Abonelik için Dizin değiştirilmiştir ve bir başarı iletisi alırsınız.</span><span class="sxs-lookup"><span data-stu-id="888f9-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="888f9-129">Yeni dizine gitmek için *Dizin* değiştiriciyi kullanın.</span><span class="sxs-lookup"><span data-stu-id="888f9-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="888f9-130">Her şeyin düzgün görünmesi 10 dakika kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="888f9-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="888f9-131">**Önerilen belgeler**</span><span class="sxs-lookup"><span data-stu-id="888f9-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="888f9-132">Azure aboneliğinin sahipliğini aktarma</span><span class="sxs-lookup"><span data-stu-id="888f9-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="888f9-133">Kaynakları yeni kaynak grubuna veya aboneliğe taşıma</span><span class="sxs-lookup"><span data-stu-id="888f9-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="888f9-134">Azure portalını kullanarak kaynakları yönetme</span><span class="sxs-lookup"><span data-stu-id="888f9-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
