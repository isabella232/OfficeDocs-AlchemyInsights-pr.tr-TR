---
title: Grup eşitlemesi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256914"
---
# <a name="group-sync"></a><span data-ttu-id="cad38-102">Grup eşitlemesi</span><span class="sxs-lookup"><span data-stu-id="cad38-102">Group sync</span></span>

<span data-ttu-id="cad38-103">Bu makalede, grup eşitlemesi hakkında yol gösterici bilgi bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cad38-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="cad38-104">Genel yönetici veya grup sahibi grup özelliklerini değiştireyene veya Azure portala üye ekleyene veya sahip atayamıyorsa, grubun yetkili kaynağının, genel yönetici veya grup sahibinin grubu değiştirmesi için Azure Active Directory (Azure AD) olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="cad38-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="cad38-105">Azure AD'de eşitlenen bir grubu silmeyi denemeden önce, hatalardan kaçınmak için tüm atanmış [lisansları sildikten](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) emin olun.</span><span class="sxs-lookup"><span data-stu-id="cad38-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="cad38-106">Kullanıcıları, grupları ve kişileri eşitlemeyi anlamak [için, Azure AD Connect Eşitleme'ye](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)bakın ve AD Connect kullanarak perm gruplarını eşitlemek için şirket içi grubu Azure AD Connect kullanarak [Azure'a](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) eşitlemeyi izleyin.</span><span class="sxs-lookup"><span data-stu-id="cad38-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="cad38-107">Eşitleme sırasında sık [karşılaşılan hataları gidermek için eşitleme](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) sırasında oluşan Hataları Giderme kılavuzuna bakın.</span><span class="sxs-lookup"><span data-stu-id="cad38-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

