---
title: Azure Faturalandırma sahipliğini aktarma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922173"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="99698-102">Azure Faturalandırma sahipliğini aktarma</span><span class="sxs-lookup"><span data-stu-id="99698-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="99698-103">Aktarmak istediğiniz aboneliğin bulunduğu faturalandırma hesabının Yöneticisi olarak [Azure portalında](https://portal.azure.com/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="99698-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="99698-104">Yönetici olduğunuzdan emin değilseniz veya kim olduğunu belirlemeniz gerekiyorsa, [Hesap faturalandırma yöneticisini belirleme](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="99698-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="99698-105">**Maliyet yönetimi + faturalamayla** arama yapın.</span><span class="sxs-lookup"><span data-stu-id="99698-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="99698-106">Sol bölmeden **abonelikler** 'i seçin.</span><span class="sxs-lookup"><span data-stu-id="99698-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="99698-107">Erişime bağlı olarak, bir faturalandırma kapsamı ve ardından **abonelikler** veya **Azure abonelikleri** 'ni seçmeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="99698-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="99698-108">Aktarmak istediğiniz aboneliğin **Faturalama sahibini aktarma** seçeneğini belirleyin</span><span class="sxs-lookup"><span data-stu-id="99698-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="99698-109">Aboneliğin yeni sahibi olacak hesabın faturalama yöneticisi olan bir kullanıcının e-posta adresini girin ve ardından **aktarım isteği gönder** 'i seçin</span><span class="sxs-lookup"><span data-stu-id="99698-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="99698-110">Kullanıcı, aktarım isteğinizi gözden geçirmeniz için yönergeler içeren bir e-posta alır.</span><span class="sxs-lookup"><span data-stu-id="99698-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="99698-111">Aktarım isteğini onaylamak için kullanıcı e-postadaki bağlantıyı seçer ve yönergeleri izler.</span><span class="sxs-lookup"><span data-stu-id="99698-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="99698-112">**Not** : aboneliğinizin fatura sahipliğini başka BIR Azure AD kiracısındaki bir kullanıcının hesabına aktarırsanız, abonelikteki kaynakları yönetmek için tüm [rol tabanlı ERIŞIM denetimi (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)atamaları kalıcı olarak kaldırılır.</span><span class="sxs-lookup"><span data-stu-id="99698-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="99698-113">Yalnızca yeni sahibin abonelikteki kaynakları yönetme erişimi olur.</span><span class="sxs-lookup"><span data-stu-id="99698-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="99698-114">Daha fazla bilgi için, [başka bir Azure AD kiracısındaki bir kullanıcıya abonelik aktarma](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="99698-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="99698-115">**Önerilen belgeler**</span><span class="sxs-lookup"><span data-stu-id="99698-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="99698-116">Azure aboneliğinin fatura sahipliğini başka bir hesaba aktarma</span><span class="sxs-lookup"><span data-stu-id="99698-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="99698-117">Bir Azure aboneliği için fatura sahipliğini aktarma hakkında</span><span class="sxs-lookup"><span data-stu-id="99698-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="99698-118">Visual Studio, Microsoft Iş ortağı ağı (MPN) ve siz kullandıkça öde dev/test abonelikleri aktarılıyor</span><span class="sxs-lookup"><span data-stu-id="99698-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="99698-119">Sahiplik aktarma SSS</span><span class="sxs-lookup"><span data-stu-id="99698-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="99698-120">Aktarım sahipliği sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="99698-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
