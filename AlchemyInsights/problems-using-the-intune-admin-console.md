---
title: Intune yönetici konsolu kullanarak sorunlar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555881"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="e9569-102">Intune yönetici konsolu kullanarak sorunlar</span><span class="sxs-lookup"><span data-stu-id="e9569-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="e9569-103">**Intune yönetici portalında gezinirken "Erişim reddedildi".**</span><span class="sxs-lookup"><span data-stu-id="e9569-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="e9569-104">Bir Intune özel rolün üyesiyseniz, hesabınıza bir Intune veya Enterprise Mobility Suite (EMS) lisansının atandığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="e9569-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="e9569-105">Aygıtları yönetmek için Configuration Manager kullanıyorsanız, Configuration Manager MDM için Intune kullanıcı koleksiyonunun bir parçası olmadığınızı doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="e9569-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="e9569-106">Intune rolleri bıçak çağınızda uygun rol tabanlı yönetim denetimi (RBAC) izinlerinin size atandığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="e9569-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="e9569-107">Kullanılan grubun dağıtım listesi olmadığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="e9569-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="e9569-108">Azure portalındaki Intune yalnızca Azure Etkin Dizin güvenlik gruplarına ait kullanıcı hesaplarını destekler.</span><span class="sxs-lookup"><span data-stu-id="e9569-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="e9569-109">Gruplarınızı Azure portalı > **Intune**  >  **Grupları'nda**veya Azure portalında Azure Active Directory > gözden **geçirin.**</span><span class="sxs-lookup"><span data-stu-id="e9569-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="e9569-110">**Kullanıcı atanan Intune rolü için çok fazla izine sahiptir**</span><span class="sxs-lookup"><span data-stu-id="e9569-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="e9569-111">Kullanıcıya **Verilen**  >  izinleri gözden geçirmek için**Intune Intune**  >  **rolleriBenim izinleri**  >  **Dışa aktarın** gidin tavsiye edin.</span><span class="sxs-lookup"><span data-stu-id="e9569-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="e9569-112">**Bir role bir kapsam grubu ekledim, ancak bu roldeki kullanıcılar hala diğer kullanıcıları veya aygıtları görür.**</span><span class="sxs-lookup"><span data-stu-id="e9569-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="e9569-113">Kapsam grupları kullanıcıları veya aygıtları filtrelemez.</span><span class="sxs-lookup"><span data-stu-id="e9569-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="e9569-114">Kapsam grupları:</span><span class="sxs-lookup"><span data-stu-id="e9569-114">Scope groups:</span></span>

- <span data-ttu-id="e9569-115">Kullanıcıların ilkeleri veya uygulamaları kimlere atayabileceğini sınırlayın.</span><span class="sxs-lookup"><span data-stu-id="e9569-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="e9569-116">Aygıtlarda yalnızca belirli kullanıcıların uzak görevleri çalıştırabilmelerine izin verin.</span><span class="sxs-lookup"><span data-stu-id="e9569-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="e9569-117">Kapsam grupları hakkında daha fazla bilgi için [Microsoft Intune ile Rol tabanlı erişim denetimi (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)'a bakın.</span><span class="sxs-lookup"><span data-stu-id="e9569-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="e9569-118">**Ben bir Intune rolü ne bir kullanıcı ekledi ama yine de Intune yönetici konsolu tam erişime sahip.**</span><span class="sxs-lookup"><span data-stu-id="e9569-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="e9569-119">Azure portalındaki Intune > **Kullanıcılar'a** gidin ve kullanıcının Azure portalında aşağıdaki rollerden hiçbirine atanmadığını doğrulayın:</span><span class="sxs-lookup"><span data-stu-id="e9569-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="e9569-120">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="e9569-120">Global administrator</span></span>
- <span data-ttu-id="e9569-121">Intune servis yöneticisi</span><span class="sxs-lookup"><span data-stu-id="e9569-121">Intune service administrator</span></span>
- <span data-ttu-id="e9569-122">SharePoint yöneticisi</span><span class="sxs-lookup"><span data-stu-id="e9569-122">SharePoint administrator</span></span>

<span data-ttu-id="e9569-123">Daha fazla bilgi için [Microsoft Intune ile Rol tabanlı erişim denetimine (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)bakın.</span><span class="sxs-lookup"><span data-stu-id="e9569-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="e9569-124">**Erişim Sorunları**</span><span class="sxs-lookup"><span data-stu-id="e9569-124">**Access Issues**</span></span>

<span data-ttu-id="e9569-125">Daha fazla bilgi için [bkz.](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)</span><span class="sxs-lookup"><span data-stu-id="e9569-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>