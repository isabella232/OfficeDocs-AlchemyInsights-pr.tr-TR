---
title: Yedek kullanıcıyı şirket içi sunucudan silme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198584"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Yedek kullanıcıyı şirket içi sunucudan silme

Yetim bir kullanıcıyı kaldırmak için aşağıdaki adımları izleyin:

1. [Azure Active Directory ile karma kimlik nedir?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Dizin eşitlemesi doğrulamak için Azure [Etkin Dizini ile karma kimlik nedir?](https://technet.microsoft.com/library/jj151797.aspx)

3. Eşitleme işlevleri doğru yse, ancak Active Directory nesne silme Azure AD'ye yayınlanmiyorsa, Windows PowerShell cmdlets için aşağıdaki Azure Etkin Dizin Modülünden birini kullanarak kullanılan ürünü n

    Kaldır-MsolContact  
    Kaldırma-MsolGroup  
    Kaldırma-MsolUser

    Örneğin, dizin eşitlemesi kullanılarak oluşturulan, ilk olarak oluşturulan kullanıcı kimliği john.smith@contoso.com kaldırmak için cmdlet'i çalıştırın:

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com