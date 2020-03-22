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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="37285-102">Outlook ortak klasörlere bağlanamıyor</span><span class="sxs-lookup"><span data-stu-id="37285-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="37285-103">Ortak klasör erişimi bazı kullanıcılar için çalışmıyorsa, aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="37285-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="37285-104">EXO PowerShell'e bağlanın ve sorunlu kullanıcı hesabındaki DefaultPublicFolderMailbox parametresini çalışan bir kullanıcı hesabındaki parametreyle eşleşecek şekilde yapılandırın.</span><span class="sxs-lookup"><span data-stu-id="37285-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="37285-105">Örnek:</span><span class="sxs-lookup"><span data-stu-id="37285-105">Example:</span></span>

<span data-ttu-id="37285-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EtkiliPublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="37285-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="37285-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<değeri önceki komut></span><span class="sxs-lookup"><span data-stu-id="37285-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="37285-108">Değişikliğin etkili olması için en az bir saat bekleyin.</span><span class="sxs-lookup"><span data-stu-id="37285-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="37285-109">Sorun devam ederse, Outlook'u kullanarak ortak klasör erişim sorunlarını gidermek için lütfen [bu yordamı](https://aka.ms/pfcte) izleyin.</span><span class="sxs-lookup"><span data-stu-id="37285-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>