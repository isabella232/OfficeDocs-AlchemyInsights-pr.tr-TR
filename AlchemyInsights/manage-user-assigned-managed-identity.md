---
title: Kullanıcıya atanan yönetilen kimliği yönetme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8211"
- "9003230"
ms.openlocfilehash: a44cb484b6d89e6d5f67b2900c38dde3610b0e23
ms.sourcegitcommit: 23e778f7414e5f1a98cc786146fe76d622b458bc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177780"
---
# <a name="manage-a-user-assigned-managed-identity"></a><span data-ttu-id="138ab-102">Kullanıcıya atanan yönetilen kimliği yönetme</span><span class="sxs-lookup"><span data-stu-id="138ab-102">Manage a user-assigned managed identity</span></span>

<span data-ttu-id="138ab-103">Kullanıcıya atanan yönetilen kimliğin yönetimi şunları içerir:</span><span class="sxs-lookup"><span data-stu-id="138ab-103">The management of a user-assigned managed identity involves:</span></span>

- <span data-ttu-id="138ab-104">Kullanıcıya atanan yönetilen kimliğe rol atama</span><span class="sxs-lookup"><span data-stu-id="138ab-104">Assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="138ab-105">Kullanıcıya atanan yönetilen kimliği silme</span><span class="sxs-lookup"><span data-stu-id="138ab-105">Deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="138ab-106">Kullanıcıya atanan yönetilen kimliği listeleme</span><span class="sxs-lookup"><span data-stu-id="138ab-106">Listing a user-assigned managed identity</span></span>

<span data-ttu-id="138ab-107">Yukarıda sözü geçen görevler hakkında daha fazla bilgi için aşağıdaki makalelere bakın:</span><span class="sxs-lookup"><span data-stu-id="138ab-107">For more information on the tasks mentioned above, see the following articles:</span></span>

- <span data-ttu-id="138ab-108">[Kullanıcıya atanan yönetilen kimlik oluşturma](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - kullanıcıya atanan yönetilen kimliğe rol atamak için</span><span class="sxs-lookup"><span data-stu-id="138ab-108">[How to create a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="138ab-109">[Kullanıcıya atanan yönetilen kimliği silme](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - kullanıcıya atanan yönetilen kimliği silmek için</span><span class="sxs-lookup"><span data-stu-id="138ab-109">[How to delete a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="138ab-110">[Kullanıcıya atanan yönetilen kimliği listeleme](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - kullanıcıya atanan yönetilen kimliği listeleme</span><span class="sxs-lookup"><span data-stu-id="138ab-110">[How to list a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for listing a user-assigned managed identity</span></span>

> [!NOTE]
> <span data-ttu-id="138ab-111">Yönetilen Kimlik Katkıda Bulunan rol **atamanız olup olmadığını** doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="138ab-111">Verify whether you have the **Managed Identity Contributor** role assignment.</span></span> <span data-ttu-id="138ab-112">Kullanıcıya atanan yönetilen kimlikleri oluşturmak/silmek için bu rol ataması gereklidir.</span><span class="sxs-lookup"><span data-stu-id="138ab-112">That role assignment is required for creating/deleting user-assigned managed identities.</span></span>
