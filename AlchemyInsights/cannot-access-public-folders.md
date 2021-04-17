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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="edbee-102">Outlook ortak klasörlere bağlanamıyor</span><span class="sxs-lookup"><span data-stu-id="edbee-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="edbee-103">Ortak klasör erişimi bazı kullanıcılarda çalışmıyorsa, şunları deneyin:</span><span class="sxs-lookup"><span data-stu-id="edbee-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="edbee-104">EXO PowerShell'e bağlanın ve sorun kullanıcı hesabında DefaultPublicFolderMailbox parametresini, çalışan bir kullanıcı hesabıdaki parametreyle eş olacak şekilde yapılandırın.</span><span class="sxs-lookup"><span data-stu-id="edbee-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="edbee-105">Örnek: </span><span class="sxs-lookup"><span data-stu-id="edbee-105">Example:</span></span>

<span data-ttu-id="edbee-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="edbee-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="edbee-107">Set-Mailbox User -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="edbee-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="edbee-108">Değişikliğin etkili olacak şekilde değişmesi için en az bir saat bekleyin.</span><span class="sxs-lookup"><span data-stu-id="edbee-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="edbee-109">Sorun devam ederse Outlook'u kullanarak [ortak klasör](https://aka.ms/pfcte) erişimi sorunlarını gidermek için lütfen bu yordamı izleyin.</span><span class="sxs-lookup"><span data-stu-id="edbee-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="edbee-110">**Outlook'u kullanarak ortak klasörlere hangi kullanıcıların eriş erişeni kontrol etmek için:**</span><span class="sxs-lookup"><span data-stu-id="edbee-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="edbee-111"><mailboxname>Set-CASMailbox -PublicFolderClientAccess $true veya $false</span><span class="sxs-lookup"><span data-stu-id="edbee-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="edbee-112">$true: Kullanıcıların Outlook'ta ortak klasörlere erişmesine izin verme</span><span class="sxs-lookup"><span data-stu-id="edbee-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="edbee-113">$false: Outlook'ta kullanıcının ortak klasörlere erişimini engelin.</span><span class="sxs-lookup"><span data-stu-id="edbee-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="edbee-114">Bu, varsayılan değerdir.</span><span class="sxs-lookup"><span data-stu-id="edbee-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="edbee-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="edbee-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="edbee-116">**Not** Bu yordam, yalnızca Windows istemcileri için Outlook masaüstü ile bağlantıları kontrol eder.</span><span class="sxs-lookup"><span data-stu-id="edbee-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="edbee-117">Bir kullanıcı OWA veya Mac için Outlook kullanarak ortak klasörlere erişmeye devam ediyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="edbee-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="edbee-118">Daha fazla bilgi için [bkz. Outlook'ta Denetimli Ortak Klasörlere Denetimli Bağlantılar için Destek Duyurma.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="edbee-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>