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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="df6dd-102">Outlook ortak klasörlere bağlanamıyor</span><span class="sxs-lookup"><span data-stu-id="df6dd-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="df6dd-103">Ortak klasör erişimi birkaç kullanıcı için çalışmıyorsa, aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="df6dd-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="df6dd-104">EXO PowerShell'e bağlanın ve sorunlu kullanıcı hesabındaki DefaultPublicFolderMailbox'ı çalışan bir kullanıcı hesabında eşleşecek şekilde yapılandırın.</span><span class="sxs-lookup"><span data-stu-id="df6dd-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="df6dd-105">Örnek:</span><span class="sxs-lookup"><span data-stu-id="df6dd-105">Example:</span></span>

<span data-ttu-id="df6dd-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EtkiliPublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="df6dd-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="df6dd-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<değeri önceki komut></span><span class="sxs-lookup"><span data-stu-id="df6dd-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="df6dd-108">Değişikliğin etkili olması için en az bir saat bekleyin.</span><span class="sxs-lookup"><span data-stu-id="df6dd-108">Wait at least one hour for the change to take effect.</span></span>