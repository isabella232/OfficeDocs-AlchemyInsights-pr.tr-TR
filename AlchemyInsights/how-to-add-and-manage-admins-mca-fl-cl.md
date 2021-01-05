---
title: Yöneticileri ekleme ve yönetme
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
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755531"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="59a03-102">Yöneticileri ekleme ve yönetme</span><span class="sxs-lookup"><span data-stu-id="59a03-102">How to add and manage admins</span></span>

<span data-ttu-id="59a03-103">Sorun açıklamanızı temel alarak sizin için bir çözüm bulduk.</span><span class="sxs-lookup"><span data-stu-id="59a03-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="59a03-104">Çoğu müşteri, belgelerimizi takip ettikten sonra sorununu kendi başınıza çözümlerler.</span><span class="sxs-lookup"><span data-stu-id="59a03-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="59a03-105">Microsoft Müşteri Anlaşmasında (MCA) faturalama hesabınızı yönetmek için, istediğiniz erişim düzeyiyle farklı roller kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="59a03-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="59a03-106">Bu roller, kaynaklarınızı denetlemenize yardımcı olan yerleşik Azure hizmet rollerine ek olarak sağlanır.</span><span class="sxs-lookup"><span data-stu-id="59a03-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="59a03-107">**Azure portalında faturalandırma rolleri eklemek için:**</span><span class="sxs-lookup"><span data-stu-id="59a03-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="59a03-108">[Azure portalında](https://portal.azure.com/)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="59a03-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="59a03-109">*Maliyet yönetimi ve faturalamayı* arayın.</span><span class="sxs-lookup"><span data-stu-id="59a03-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="59a03-110">Erişim vermek istediğiniz fatura hesabı, fatura profili veya fatura bölümü gibi bir kapsamda erişim denetimini (ıAM) seçin.</span><span class="sxs-lookup"><span data-stu-id="59a03-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="59a03-111">Erişim denetimi (ıAM) sayfası, bu kapsam için her role atanmış olan Kullanıcı ve grupları listeler.</span><span class="sxs-lookup"><span data-stu-id="59a03-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="59a03-112">Kullanıcıya erişim vermek için, sayfanın başından **Ekle** 'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="59a03-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="59a03-113">*Rol* açılan listesinde bir rol seçin.</span><span class="sxs-lookup"><span data-stu-id="59a03-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="59a03-114">Erişim vermek istediğiniz kullanıcının e-posta adresini girin.</span><span class="sxs-lookup"><span data-stu-id="59a03-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="59a03-115">Rolü atamak için **Kaydet** 'i seçin.</span><span class="sxs-lookup"><span data-stu-id="59a03-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="59a03-116">Bir kullanıcının erişimini kaldırmak için, kaldırmak istediğiniz rol atamasını içeren kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="59a03-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="59a03-117">**Kaldır**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="59a03-117">Select **Remove**.</span></span>

<span data-ttu-id="59a03-118">**Önerilen Belgeler**</span><span class="sxs-lookup"><span data-stu-id="59a03-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="59a03-119">Faturalandırma rolü tanımları</span><span class="sxs-lookup"><span data-stu-id="59a03-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="59a03-120">Faturalandırma hesabı rolleri ve görevleri</span><span class="sxs-lookup"><span data-stu-id="59a03-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="59a03-121">MCA Faturalandırma hesabınızla çalışmaya başlama</span><span class="sxs-lookup"><span data-stu-id="59a03-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="59a03-122">Microsoft Müşteri sözleşmesine erişimi denetleme</span><span class="sxs-lookup"><span data-stu-id="59a03-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
