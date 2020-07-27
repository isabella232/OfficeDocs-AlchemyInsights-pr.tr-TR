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
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Outlook'a eklenti eklerken birden çok kullanıcı Access Reddedildi hatası na sayılsın

Kuruluşunuzdaki hangi yöneticilerin Outlook eklentilerini yükleme ve yönetme izinlerine sahip olduğunu belirtebilirsiniz. Ayrıca, kuruluşunuzdaki hangi kullanıcıların kendi kullanımları için eklentileri yükleme ve yönetme iznine sahip olduğunu da belirtebilirsiniz.

Ayrıntılar için bkz. [Outlook eklentilerini yükleyip yönetebilecek yöneticileri ve kullanıcıları belirtin.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)

Bir kullanıcı için izinleri başarıyla atadığınızı doğrulamak için, doğrulamak için rolün adı ile değiştirin <Role Name> ve Exchange Online PowerShell'de aşağıdaki komutu çalıştırın:

Get-ManagementRoleAssignment -Role " <Role Name> -GetEffectiveUsers

Bu örnek, kuruluş için Office Mağazası'ndan eklentiler yüklemek için kime izin ler atadığınızı nasıl doğrulayabileceğinizi gösterir.

Powershell

-Role "Org Marketplace Apps" -GetEffectiveUsers

Sonuçlarda, Get-ManagementRoleAssignment, Etkili Kullanıcılar sütunundaki girişleri gözden geçirin.

Ayrıntılı sözdizimi ve parametre bilgileri için [bkz.](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)
 