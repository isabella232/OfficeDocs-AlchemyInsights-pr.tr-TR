---
title: Outlook'ta eklentileri görmeyen tek kullanıcı
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198223"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="2bbec-102">Outlook'ta eklentileri görmeyen tek kullanıcı</span><span class="sxs-lookup"><span data-stu-id="2bbec-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="2bbec-103">Kullanıcı, doğru AppsForOfficeEtkin parametreye sahip olmayan bir rolün parçası olabilir.</span><span class="sxs-lookup"><span data-stu-id="2bbec-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="2bbec-104">Doğru rolün kullanıcıyla ilişkilendirilip ilişkilendirilmesi gerektiğini öğrenmek için bu cmdlet'i çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="2bbec-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="2bbec-105">Al-ManagementRoleAssignment -RoleAssignee user@domain.com -$false Atama | Biçim-Tablo -Otomatik Rol,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="2bbec-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="2bbec-106">Daha fazla bilgi için bkz. [Outlook eklentilerini yükleyip yönetebilecek yöneticileri ve kullanıcıları belirtin.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)</span><span class="sxs-lookup"><span data-stu-id="2bbec-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
