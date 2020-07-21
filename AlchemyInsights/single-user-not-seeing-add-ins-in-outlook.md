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
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Outlook'ta eklentileri görmeyen tek kullanıcı

Kullanıcı, doğru AppsForOfficeEtkin parametreye sahip olmayan bir rolün parçası olabilir. Doğru rolün kullanıcıyla ilişkilendirilip ilişkilendirilmesi gerektiğini öğrenmek için bu cmdlet'i çalıştırın:

Al-ManagementRoleAssignment -RoleAssignee user@domain.com -$false Atama | Biçim-Tablo -Otomatik Rol,RoleAssigneeName,RoleAssigneeType

Daha fazla bilgi için bkz. [Outlook eklentilerini yükleyip yönetebilecek yöneticileri ve kullanıcıları belirtin.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)
