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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996650"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ortak klasörlere bağlanamıyor

Ortak klasör erişimi bazı kullanıcılarda çalışmıyorsa, şunları deneyin:

Bağlan sonra EXO PowerShell'e tıklayın ve sorun kullanıcı hesabında DefaultPublicFolderMailbox parametresini çalışan kullanıcı hesabıdaki parametreyle eş olacak şekilde yapılandırın.

Örneğin:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox User -DefaultPublicFolderMailbox \<value from previous command>

Değişikliğin etkili olacak şekilde değişmesi için en az bir saat bekleyin.

Sorun devam ederse, [](https://aka.ms/pfcte) Outlook kullanarak ortak klasör erişimi sorunlarını gidermek için lütfen bu Outlook.
 
**Hangi kullanıcıların ortak klasörlere erişeni, Outlook:**

1.  <mailboxname>Set-CASMailbox -PublicFolderClientAccess $true veya $false  
      
    $true: Kullanıcıların e-postada ortak klasörlere erişmesine izin Outlook  
      
    $false: Bir klasörde kullanıcının ortak klasörlere erişimini Outlook. Bu, varsayılan değerdir.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Not** Bu yordam, yalnızca Outlook Outlook istemcileri için Windows denetime sahiptir. Bir kullanıcı OWA veya posta hesabı kullanarak ortak klasörlere erişmeye Mac için Outlook.
 
Daha fazla bilgi için [bkz. Denetimli Ortak](https://aka.ms/controlpf)Klasörlere Denetimli Bağlantılar için Destek Outlook.