---
title: Gözden geçirme
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7767"
ms.openlocfilehash: b2ba50c4f8e667f81b638ba480fa846e149c3d43
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014994"
---
# <a name="access-reviews"></a><span data-ttu-id="24289-102">Gözden geçirme</span><span class="sxs-lookup"><span data-stu-id="24289-102">Access reviews</span></span>

1. <span data-ttu-id="24289-103">**Access Incelemelerini etkinleştir**: yeni bir Access paketi oluştururken veya varolan bir Access paketini düzenlediğinizde İncelemeleri etkinleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="24289-103">**Enable Access Reviews**: You can enable reviews when you create a new access package or edit an existing access package.</span></span> <span data-ttu-id="24289-104">[Azure AD hak yönetimi 'nde bir Access paketinin erişim Incelemesini oluşturma](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) Access paketlerinin erişim incelemelerini nasıl etkinleştireceğiniz açıklanır.</span><span class="sxs-lookup"><span data-stu-id="24289-104">[Create an access review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) describes how to enable access reviews of access packages.</span></span>

1. <span data-ttu-id="24289-105">**Erişimi gözden geçir**: Azure AD hak yönetimi, kuruluşların gruplara, uygulamalara ve SharePoint sitelerine erişimi nasıl yönetebileceğinizi basitleştirir.</span><span class="sxs-lookup"><span data-stu-id="24289-105">**Review Access**: Azure AD entitlement management simplifies how enterprises manage access to groups, applications, and SharePoint sites.</span></span> <span data-ttu-id="24289-106">[Azure AD hak yönetiminde bir Access paketinin erişimini gözden geçirme](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) bir Access paketine atanmış gözden geçiren olarak atanan diğer kullanıcılar için Access incelemelerini nasıl gerçekleştirebileceğinizi açıklar.</span><span class="sxs-lookup"><span data-stu-id="24289-106">[Review access of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) describes how to perform access reviews for other users that are assigned to an access package as a designated reviewer.</span></span>

1. <span data-ttu-id="24289-107">**Kendinize yönelik erişimi gözden geçirin**: [Azure AD hak yönetimi 'nde bir Access paketini kendi başına gözden geçirme](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) , kullanıcının atanmış erişim paketlerini kendi kendine nasıl gözden geçirebileceğinizi açıklar.</span><span class="sxs-lookup"><span data-stu-id="24289-107">**Review Access for Yourself**: [Self-review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) describes how a user does a self-review of their assigned access package(s).</span></span>

1. <span data-ttu-id="24289-108">Çoğu durumda son kullanıcılar, **erişim panelinde** yanıtının bekleyen bir gözden geçirisini bulacaktır.</span><span class="sxs-lookup"><span data-stu-id="24289-108">In most cases, end users will find a review pending their response in the **Access Panel**.</span></span> <span data-ttu-id="24289-109">Bu yalnızca grupların ve uygulamaların incelemelerinin değil, roller için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="24289-109">This is only applicable to reviews of Groups and Applications, not Roles.</span></span> <span data-ttu-id="24289-110">Rollerin tüm erişim Incelemelerinde, son kullanıcılar gözden geçirmeyi tamamlamak için Azure AD ayrıcalıklı kimlik yönetimi 'ne (PıM) gitmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="24289-110">For all Access Reviews of roles, end users must navigate to Azure AD Privileged Identity Management (PIM) to complete their review.</span></span>

    1. <span data-ttu-id="24289-111">Azure portalında oturum açın.</span><span class="sxs-lookup"><span data-stu-id="24289-111">Logon to the Azure portal.</span></span>
    2. <span data-ttu-id="24289-112">Azure AD PıM 'ye gidin.</span><span class="sxs-lookup"><span data-stu-id="24289-112">Navigate to Azure AD PIM.</span></span>
    3. <span data-ttu-id="24289-113">Sol gezinti bölmesinde, **görevleri**  >  **gözden geçir**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="24289-113">In the left navigation pane, select **Tasks** > **Review access**.</span></span>
    
<span data-ttu-id="24289-114">Daha fazla bilgi için bkz.:</span><span class="sxs-lookup"><span data-stu-id="24289-114">For more information, see:</span></span>

- [<span data-ttu-id="24289-115">PıM 'deki Azure AD dizini rollerimin erişim incelemesini gerçekleştirme </span><span class="sxs-lookup"><span data-stu-id="24289-115">Perform an access review of my Azure AD directory roles in PIM </span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-perform-security-review/)
- [<span data-ttu-id="24289-116">PıM 'deki Azure Resource rollerimin erişim incelemesini gerçekleştirme</span><span class="sxs-lookup"><span data-stu-id="24289-116">Perform an access review of my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-perform-access-review/)