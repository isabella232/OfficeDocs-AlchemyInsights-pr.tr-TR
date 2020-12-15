---
title: Maliyet yönetimini etkinleştirme
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
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678775"
---
# <a name="enable-cost-management"></a><span data-ttu-id="c91dd-102">Maliyet yönetimini etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="c91dd-102">Enable cost management</span></span>

<span data-ttu-id="c91dd-103">**' Kuruluşunuz için maliyetlerin devre dışı bırakıldığı ' nedir?**</span><span class="sxs-lookup"><span data-stu-id="c91dd-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="c91dd-104">Kurumsal Sözleşme (EA) veya Microsoft Customer Agreement (MCA) hesaplarını kullanan kuruluşlar, maliyet bilgilerine ve fiyatlandırma bilgilerine erişimi devre dışı bırakabilir.</span><span class="sxs-lookup"><span data-stu-id="c91dd-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="c91dd-105">Azure portalında oturum açtıktan sonra, fatura API 'Lerini kullanarak faturaları (kabul edildikten) ve kullanım ayrıntılarını kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c91dd-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="c91dd-106">**Ek kullanıcıların faturalara erişmesine izin verme**</span><span class="sxs-lookup"><span data-stu-id="c91dd-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="c91dd-107">Azure portalında **abonelikler dikey** bölümüne gidin.</span><span class="sxs-lookup"><span data-stu-id="c91dd-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="c91dd-108">**Faturaları** seçin ve ardından **faturalara erişin**.</span><span class="sxs-lookup"><span data-stu-id="c91dd-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="c91dd-109">Aboneliği kapsamlı rollerin kullanıcılarına faturaları indirme izni vermek için, ardından değişiklikleri kaydederek erişimi açın.</span><span class="sxs-lookup"><span data-stu-id="c91dd-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="c91dd-110">Hesap Yöneticisi e-posta yoluyla faturaları göndermek için de yapılandırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c91dd-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="c91dd-111">Daha fazla [bilgi edinmek için bkz.](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)</span><span class="sxs-lookup"><span data-stu-id="c91dd-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="c91dd-112">**Faturalandırma okuyucusu rolüne kullanıcı ekleme**</span><span class="sxs-lookup"><span data-stu-id="c91dd-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="c91dd-113">Azure portalında **abonelikler dikey** bölümüne gidin.</span><span class="sxs-lookup"><span data-stu-id="c91dd-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="c91dd-114">**Erişim denetimi 'ni (IAM)** seçin ve **Ekle**'yi tıklatın.</span><span class="sxs-lookup"><span data-stu-id="c91dd-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="c91dd-115">**Bir rol seçin** sayfasında **faturalandırma okuyucuyu** seçin.</span><span class="sxs-lookup"><span data-stu-id="c91dd-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="c91dd-116">Davet etmek istediğiniz kullanıcının e-postasını yazın ve daveti göndermek için **Tamam** 'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="c91dd-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="c91dd-117">Ödeme okuyucusu olarak oturum açmak için davet e-postada sağlanan yönergeleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="c91dd-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="c91dd-118">Daha fazla bilgi için bkz [.](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)</span><span class="sxs-lookup"><span data-stu-id="c91dd-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="c91dd-119">**Önerilen belgeler**</span><span class="sxs-lookup"><span data-stu-id="c91dd-119">**Recommended documents**</span></span>

- [<span data-ttu-id="c91dd-120">EA portalında DA ve AO görünümlerini etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="c91dd-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="c91dd-121">Maliyet yönetimine dahil olan maliyetler</span><span class="sxs-lookup"><span data-stu-id="c91dd-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="c91dd-122">Desteklenen Microsoft Azure teklifleri</span><span class="sxs-lookup"><span data-stu-id="c91dd-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="c91dd-123">Maliyet analizinde maliyetleri gözden geçirme</span><span class="sxs-lookup"><span data-stu-id="c91dd-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="c91dd-124">Faturalandırma bilgilerine erişim sağlama</span><span class="sxs-lookup"><span data-stu-id="c91dd-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="c91dd-125">Microsoft Müşteri sözleşmesine erişimi denetleme</span><span class="sxs-lookup"><span data-stu-id="c91dd-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






