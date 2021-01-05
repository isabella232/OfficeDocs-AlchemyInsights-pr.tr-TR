---
title: Faturaya göre Öde (Çek/tel aktarımı)
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
- "9004168"
- "7343"
ms.openlocfilehash: c4c78d634cdef711423f573439c5091befedef34
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755423"
---
# <a name="switch-to-pay-by-invoice-chequewire-transfer"></a><span data-ttu-id="cb029-102">Faturaya göre Öde (Çek/tel aktarımı)</span><span class="sxs-lookup"><span data-stu-id="cb029-102">Switch to pay by invoice (cheque/wire transfer)</span></span>

<span data-ttu-id="cb029-103">Sorun açıklamanızı temel alarak sizin için bir çözüm bulduk.</span><span class="sxs-lookup"><span data-stu-id="cb029-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="cb029-104">Çoğu müşteri, belgelerimizi takip ettikten sonra sorununu kendi başınıza çözümlerler.</span><span class="sxs-lookup"><span data-stu-id="cb029-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="cb029-105">Faturaya göre öde 'ye geçerseniz, bu, faturanızı fatura tarihinin 30 günü içinde ödeyeceğiniz anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="cb029-105">If you switch to pay by invoice, that means you will pay your bill within 30 days of the invoice date.</span></span> <span data-ttu-id="cb029-106">Azure aboneliğiniz için ödeme yapmak üzere bir Azure desteğine istek gönderin.</span><span class="sxs-lookup"><span data-stu-id="cb029-106">To become eligible to pay for your Azure subscription by invoice, submit a request to Azure support.</span></span> <span data-ttu-id="cb029-107">İsteğiniz onaylandıktan sonra, [Azure portalında](https://portal.azure.com/)fatura ödemesi için aboneliği değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cb029-107">Once your request is approved, you can switch a subscription to invoice pay in the [Azure portal](https://portal.azure.com/).</span></span>

<span data-ttu-id="cb029-108">**Daha fazla devam etmeden önce aşağıdaki gereksinimleri/fatura ödeme isteğinde bulunan sınırlamaları gözden geçirin:**</span><span class="sxs-lookup"><span data-stu-id="cb029-108">**Before you proceed further, review the following requirements/limitations on requesting invoice payment option:**</span></span>

- <span data-ttu-id="cb029-109">[Azure portalında](https://portal.azure.com/) oturum açın ve ödeme yöntemlerine gidin.</span><span class="sxs-lookup"><span data-stu-id="cb029-109">Log in to [Azure portal](https://portal.azure.com/) and navigate to payment methods.</span></span> <span data-ttu-id="cb029-110">Fatura ödemesi için önceden onaylanmış olup olmadığını denetleyin.</span><span class="sxs-lookup"><span data-stu-id="cb029-110">Check if you are already pre-approved for invoice payment.</span></span>
- <span data-ttu-id="cb029-111">Fatura ödemesi yalnızca iş hesaplarında kullanılabilir, kişisel hesaplarda kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="cb029-111">Invoice pay is only available for business accounts, not for personal accounts.</span></span>
- <span data-ttu-id="cb029-112">Fatura ödemenize geçmeden önce tüm bekleyen ücretleri ödemelisiniz.</span><span class="sxs-lookup"><span data-stu-id="cb029-112">You must pay all outstanding charges before switching to invoice pay.</span></span>
- <span data-ttu-id="cb029-113">Destek ekibi, fatura ödeme moduna uygun olup olmadığını belirlemek için hesabı gözden geçirir.</span><span class="sxs-lookup"><span data-stu-id="cb029-113">The support team will review the account to determine if it is eligible for invoice mode of payment.</span></span>
- <span data-ttu-id="cb029-114">Market üçüncü taraf hizmetleri için fatura ödeme modu desteklenmez; geçerli aboneliği Market veya üçüncü taraf hizmetlerini içeren bir faturaya geçirmek istiyorsanız, bu hizmetlerin geçiş öncesinde silinmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="cb029-114">Invoice mode of payment is not supported for marketplace 3rd party services; if you intend to switch a current subscription to an invoice that contains marketplace or 3rd party services, these services must be deleted before switching.</span></span> <span data-ttu-id="cb029-115">Gelecekteki Market Hizmetleri için önce kredi kartında ayrı bir abonelik satın alın ve ardından Market üçüncü taraf hizmetlerini satın alın veya dağıtın.</span><span class="sxs-lookup"><span data-stu-id="cb029-115">For future marketplace services, purchase a separate subscription on credit card first and then purchase or deploy marketplace 3rd party services.</span></span>
- <span data-ttu-id="cb029-116">Fatura ödemelerini değiştirdiğinizde, kredi veya banka kartı ödemesi 'ne geri dönebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cb029-116">Once you switch to invoice pay, you can't switch back to credit or debit card payment.</span></span>

<span data-ttu-id="cb029-117">*Faturaya göre ödeme yapmayı onayladıktan sonra* Azure aboneliğinizi, [Azure portalında](https://portal.azure.com/)çek veya kablo aktarımı aracılığıyla fatura ödemenize değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cb029-117">*Once you're approved to pay by invoice*, you can switch your Azure subscription to the invoice pay via cheque or wire transfer in the [Azure portal](https://portal.azure.com/).</span></span>
<span data-ttu-id="cb029-118">Bunu yapmak için:</span><span class="sxs-lookup"><span data-stu-id="cb029-118">To do that:</span></span>

1. <span data-ttu-id="cb029-119">Hesap Yöneticisi olarak [Azure portalında](https://portal.azure.com/)oturum açın   .</span><span class="sxs-lookup"><span data-stu-id="cb029-119">Sign in to the [Azure portal](https://portal.azure.com/) as the Account Administrator.</span></span> <span data-ttu-id="cb029-120"> *\*Maliyet yönetimi + faturalamayı** arayıp seçin.</span><span class="sxs-lookup"><span data-stu-id="cb029-120">Search for and select **Cost Management + Billing**.</span></span>
2. <span data-ttu-id="cb029-121">Fatura ödemesini yapmak istediğiniz aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="cb029-121">Select the subscription you would like to switch to invoice payment.</span></span> <span data-ttu-id="cb029-122">**Ödeme yöntemlerini** seçin.</span><span class="sxs-lookup"><span data-stu-id="cb029-122">Select **Payment methods**.</span></span>
3. <span data-ttu-id="cb029-123">Komut çubuğunda **faturaya göre öde** düğmesini tıklatın.</span><span class="sxs-lookup"><span data-stu-id="cb029-123">In the command bar, click the **Pay by invoice** button.</span></span>

<span data-ttu-id="cb029-124">**Önerilen Belgeler**</span><span class="sxs-lookup"><span data-stu-id="cb029-124">**Recommended Documents**</span></span>

- [<span data-ttu-id="cb029-125">Azure Faturalandırma faturanızı ve kullanım verilerinizi isteme/Indirme/görüntüleme</span><span class="sxs-lookup"><span data-stu-id="cb029-125">Request/Download/View your Azure billing invoice and usage data</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="cb029-126">Azure faturalarını doğrudan gelen kutunuza gönderin</span><span class="sxs-lookup"><span data-stu-id="cb029-126">How to email Azure invoices directly to your inbox</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="cb029-127">Faturayla öde</span><span class="sxs-lookup"><span data-stu-id="cb029-127">Pay by invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-pay-by-invoice)
- [<span data-ttu-id="cb029-128">Ayrıntılı kullanım ücretlerini anlama</span><span class="sxs-lookup"><span data-stu-id="cb029-128">Understand detailed usage charges</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-bill)
- [<span data-ttu-id="cb029-129">Faturanızın şartlarını anlama</span><span class="sxs-lookup"><span data-stu-id="cb029-129">Understand terms on your invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-invoice)
- [<span data-ttu-id="cb029-130">Sahipliği aktarma</span><span class="sxs-lookup"><span data-stu-id="cb029-130">How to transfer ownership</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer)
