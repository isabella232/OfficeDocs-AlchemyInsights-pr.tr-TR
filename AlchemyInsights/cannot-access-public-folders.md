---
title: Ortak klasörlere erişemiyor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891769"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ortak klasörlere bağlanamıyor

Ortak klasör erişimi bazı kullanıcılar için çalışmıyorsa, aşağıdakileri deneyin:

EXO PowerShell'e bağlanın ve sorunlu kullanıcı hesabındaki DefaultPublicFolderMailbox parametresini çalışan bir kullanıcı hesabındaki parametreyle eşleşecek şekilde yapılandırın.

Örnek:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EtkiliPublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<değeri önceki komut>

Değişikliğin etkili olması için en az bir saat bekleyin.

Sorun devam ederse, Outlook'u kullanarak ortak klasör erişim sorunlarını gidermek için lütfen [bu yordamı](https://aka.ms/pfcte) izleyin.