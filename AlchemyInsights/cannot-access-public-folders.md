---
title: Ortak klasörlere erişem yok
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819532"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ortak klasörlere bağlanamıyor

Ortak klasör erişimi bazı kullanıcılarda çalışmıyorsa, şunları deneyin:

EXO PowerShell'e bağlanın ve sorun kullanıcı hesabında DefaultPublicFolderMailbox parametresini, çalışan bir kullanıcı hesabıdaki parametreyle eş olacak şekilde yapılandırın.

Örnek: 

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox User -DefaultPublicFolderMailbox \<value from previous command>

Değişikliğin etkili olacak şekilde değişmesi için en az bir saat bekleyin.

Sorun devam ederse Outlook'u kullanarak [ortak klasör](https://aka.ms/pfcte) erişimi sorunlarını gidermek için lütfen bu yordamı izleyin.
 
**Outlook'u kullanarak ortak klasörlere hangi kullanıcıların eriş erişeni kontrol etmek için:**

1.  <mailboxname>Set-CASMailbox -PublicFolderClientAccess $true veya $false  
      
    $true: Kullanıcıların Outlook'ta ortak klasörlere erişmesine izin verme  
      
    $false: Outlook'ta kullanıcının ortak klasörlere erişimini engelin. Bu, varsayılan değerdir.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Not** Bu yordam, yalnızca Windows istemcileri için Outlook masaüstü ile bağlantıları kontrol eder. Bir kullanıcı OWA veya Mac için Outlook kullanarak ortak klasörlere erişmeye devam ediyor olabilir.
 
Daha fazla bilgi için [bkz. Outlook'ta Denetimli Ortak Klasörlere Denetimli Bağlantılar için Destek Duyurma.](https://aka.ms/controlpf)