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
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Outlook'ta eklentileri görmeyen birden çok kullanıcı

Outlook eklentilerini sınarsanız ve hiçbiri görünmüyorsa, ilk sorun giderme adımı olarak, _AppsForOfficeEtkin_ parametresini sorgulamak için **Get-OrganizationConfig** PowerShell cmdlet'ini kullanın. Sorgu **False**değerini döndürürse, bu parametreyi **Set-OrganizationConfig** cmdlet'i kullanarak **True** olarak ayarlayın, bu nedenle eklentiler beklendiği gibi görünür.

_AppsForOfficeEtkin_ parametrenin **False**olarak ayarlanmasını önermiyoruz. **False** değeri, yukarıdaki Yönetim ve Kullanıcı rol ayarlarının tümünün geçersiz kılar ve yeni uygulamaların kuruluştaki herhangi bir kullanıcı tarafından etkinleştirilmesini engeller.

Daha fazla bilgi için bkz. [Outlook eklentilerini yükleyip yönetebilecek yöneticileri ve kullanıcıları belirtin.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)