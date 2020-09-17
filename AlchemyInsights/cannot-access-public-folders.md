---
title: Ortak klasörlere erişilemiyor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812567"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ortak klasörlere bağlanamıyor

Bazı kullanıcılar için ortak klasör erişimi çalışmıyorsa, aşağıdakileri deneyin:

EXO PowerShell 'e bağlanın ve sorunlu Kullanıcı hesabındaki DefaultPublicFolderMailbox parametresini çalışan bir kullanıcı hesabındaki parametreyle eşleşecek şekilde yapılandırın.

Örnekteki

Get-posta kutusu WorkingUser | ft defaultpublicfoldermailbox, efekt

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Değişikliğin geçerlilik kazanması için en az bir saat bekleyin.

Sorun devam ederse, Outlook 'U kullanarak ortak klasör erişimi sorunlarını gidermek için lütfen [Bu yordamı](https://aka.ms/pfcte) izleyin.
 
**Hangi kullanıcıların Outlook kullanan ortak klasörlere erişebileceğini denetlemek için**:

1.  Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true veya $false kullanma  
      
    $true: Outlook 'ta kullanıcıların ortak klasörlerine erişmesine Izin verme  
      
    $false: Outlook 'ta ortak klasörlere Kullanıcı erişimini önleyin. Bu, varsayılan değerdir.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Not** Bu yordam yalnızca Windows için Outlook masaüstü ile bağlantıları denetleyebilir. Bir Kullanıcı OWA veya Mac için Outlook kullanarak ortak klasörlere erişmeye devam edebilir.
 
Daha fazla bilgi için, [Outlook 'Ta ortak klasörlerin denetlenen bağlantıları Için destek duyurun](https://aka.ms/controlpf).