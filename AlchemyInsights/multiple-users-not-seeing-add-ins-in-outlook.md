---
title: Outlook'ta eklentileri görmeyen birden çok kullanıcı
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
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198245"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="d74fa-102">Outlook'ta eklentileri görmeyen birden çok kullanıcı</span><span class="sxs-lookup"><span data-stu-id="d74fa-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="d74fa-103">Outlook eklentilerini sınarsanız ve hiçbiri görünmüyorsa, ilk sorun giderme adımı olarak, _AppsForOfficeEtkin_ parametresini sorgulamak için **Get-OrganizationConfig** PowerShell cmdlet'ini kullanın.</span><span class="sxs-lookup"><span data-stu-id="d74fa-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="d74fa-104">Sorgu **False**değerini döndürürse, bu parametreyi **Set-OrganizationConfig** cmdlet'i kullanarak **True** olarak ayarlayın, bu nedenle eklentiler beklendiği gibi görünür.</span><span class="sxs-lookup"><span data-stu-id="d74fa-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="d74fa-105">_AppsForOfficeEtkin_ parametrenin **False**olarak ayarlanmasını önermiyoruz.</span><span class="sxs-lookup"><span data-stu-id="d74fa-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="d74fa-106">**False** değeri, yukarıdaki Yönetim ve Kullanıcı rol ayarlarının tümünün geçersiz kılar ve yeni uygulamaların kuruluştaki herhangi bir kullanıcı tarafından etkinleştirilmesini engeller.</span><span class="sxs-lookup"><span data-stu-id="d74fa-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="d74fa-107">Daha fazla bilgi için bkz. [Outlook eklentilerini yükleyip yönetebilecek yöneticileri ve kullanıcıları belirtin.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)</span><span class="sxs-lookup"><span data-stu-id="d74fa-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>