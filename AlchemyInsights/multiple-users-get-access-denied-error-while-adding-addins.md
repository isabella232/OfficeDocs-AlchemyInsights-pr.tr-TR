---
title: Outlook'a eklenti eklerken birden çok kullanıcı Access Reddedildi hatası na sayılsın
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424178"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="0d34a-102">Outlook'a eklenti eklerken birden çok kullanıcı Access Reddedildi hatası na sayılsın</span><span class="sxs-lookup"><span data-stu-id="0d34a-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="0d34a-103">Kuruluşunuzdaki hangi yöneticilerin Outlook eklentilerini yükleme ve yönetme izinlerine sahip olduğunu belirtebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0d34a-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="0d34a-104">Ayrıca, kuruluşunuzdaki hangi kullanıcıların kendi kullanımları için eklentileri yükleme ve yönetme iznine sahip olduğunu da belirtebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0d34a-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="0d34a-105">Ayrıntılar için bkz. [Outlook eklentilerini yükleyip yönetebilecek yöneticileri ve kullanıcıları belirtin.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)</span><span class="sxs-lookup"><span data-stu-id="0d34a-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="0d34a-106">Bir kullanıcı için izinleri başarıyla atadığınızı doğrulamak için, doğrulamak için rolün adı ile değiştirin <Role Name> ve Exchange Online PowerShell'de aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="0d34a-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="0d34a-107">Get-ManagementRoleAssignment -Role " <Role Name> -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="0d34a-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="0d34a-108">Bu örnek, kuruluş için Office Mağazası'ndan eklentiler yüklemek için kime izin ler atadığınızı nasıl doğrulayabileceğinizi gösterir.</span><span class="sxs-lookup"><span data-stu-id="0d34a-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="0d34a-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="0d34a-109">PowerShell</span></span>

<span data-ttu-id="0d34a-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="0d34a-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="0d34a-111">Sonuçlarda, Get-ManagementRoleAssignment, Etkili Kullanıcılar sütunundaki girişleri gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="0d34a-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="0d34a-112">Ayrıntılı sözdizimi ve parametre bilgileri için [bkz.](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)</span><span class="sxs-lookup"><span data-stu-id="0d34a-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 