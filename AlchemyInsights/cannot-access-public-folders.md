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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959514"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ortak klasörlere bağlanamıyor

Ortak klasör erişimi birkaç kullanıcı için çalışmıyorsa, aşağıdakileri deneyin:

EXO PowerShell'e bağlanın ve sorunlu kullanıcı hesabındaki DefaultPublicFolderMailbox'ı çalışan bir kullanıcı hesabında eşleşecek şekilde yapılandırın.

Örnek:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EtkiliPublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<değeri önceki komut>

Değişikliğin etkili olması için en az bir saat bekleyin.