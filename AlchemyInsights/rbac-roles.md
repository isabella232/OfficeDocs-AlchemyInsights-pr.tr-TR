---
title: 'RBAC rolleri '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583956"
---
# <a name="rbac-rules"></a><span data-ttu-id="3b1ef-102">RBAC kuralları</span><span class="sxs-lookup"><span data-stu-id="3b1ef-102">RBAC rules</span></span>

<span data-ttu-id="3b1ef-103">İzin hatasını alırsanız:</span><span class="sxs-lookup"><span data-stu-id="3b1ef-103">If you get the permission error:</span></span> 

- <span data-ttu-id="3b1ef-104">**Nesne kimliğine sahip istemci kapsam üzerinde eylem gerçekleştirme yetkisine sahip değil (kod: Authorizationbaşarısız oldu)**: bir kaynak oluşturmaya çalıştığınızda, şu anda seçili kapsamda kaynağa yazma izni olan bir rol atanmış bir kullanıcıyla oturumunuz açık olup olmadığını denetleyin.</span><span class="sxs-lookup"><span data-stu-id="3b1ef-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="3b1ef-105">Örneğin, kaynak grubundaki sanal makineleri yönetmek için kaynak grubunda (veya üst kapsamda) [sanal makine katılımcısı](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) rolüne sahip olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="3b1ef-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="3b1ef-106">Yerleşik rollerin izinlerinin listesi için, [Azure kaynakları Için yerleşik rollere](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)bakın.</span><span class="sxs-lookup"><span data-stu-id="3b1ef-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="3b1ef-107">**Destek isteği oluşturmak için izniniz** yok: bir destek bileti oluşturmaya veya güncelleştirmeye çalıştığınızda, şu anda Microsoft. support/supportticket/Write iznine sahip bir rol atanmış olan bir kullanıcı ile oturumunuz açık olup olmadığını denetleyin; Örneğin, bu [katılımcı desteği](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="3b1ef-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="3b1ef-108">**Daha fazla rol ataması oluşturulamaz (kod: roleatamasayısı)**: rol atamayı denediğinizde, bunun yerine gruplara roller atayarak rol atamalarının sayısını azaltmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="3b1ef-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="3b1ef-109">Azure, abonelik başına en çok **2000** rol atamasını destekler.</span><span class="sxs-lookup"><span data-stu-id="3b1ef-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="3b1ef-110">Azure RBAC rolleriyle ilgili daha fazla bilgi için [Azure RBAC rollerine](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)bakın.</span><span class="sxs-lookup"><span data-stu-id="3b1ef-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
