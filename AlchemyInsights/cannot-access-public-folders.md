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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="e3f3a-102">Outlook ortak klasörlere bağlanamıyor</span><span class="sxs-lookup"><span data-stu-id="e3f3a-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="e3f3a-103">Bazı kullanıcılar için ortak klasör erişimi çalışmıyorsa, aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="e3f3a-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="e3f3a-104">EXO PowerShell 'e bağlanın ve sorunlu Kullanıcı hesabındaki DefaultPublicFolderMailbox parametresini çalışan bir kullanıcı hesabındaki parametreyle eşleşecek şekilde yapılandırın.</span><span class="sxs-lookup"><span data-stu-id="e3f3a-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="e3f3a-105">Örnekteki</span><span class="sxs-lookup"><span data-stu-id="e3f3a-105">Example:</span></span>

<span data-ttu-id="e3f3a-106">Get-posta kutusu WorkingUser | ft defaultpublicfoldermailbox, efekt</span><span class="sxs-lookup"><span data-stu-id="e3f3a-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="e3f3a-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="e3f3a-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="e3f3a-108">Değişikliğin geçerlilik kazanması için en az bir saat bekleyin.</span><span class="sxs-lookup"><span data-stu-id="e3f3a-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="e3f3a-109">Sorun devam ederse, Outlook 'U kullanarak ortak klasör erişimi sorunlarını gidermek için lütfen [Bu yordamı](https://aka.ms/pfcte) izleyin.</span><span class="sxs-lookup"><span data-stu-id="e3f3a-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="e3f3a-110">**Hangi kullanıcıların Outlook kullanan ortak klasörlere erişebileceğini denetlemek için**:</span><span class="sxs-lookup"><span data-stu-id="e3f3a-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="e3f3a-111">Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true veya $false kullanma</span><span class="sxs-lookup"><span data-stu-id="e3f3a-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="e3f3a-112">$true: Outlook 'ta kullanıcıların ortak klasörlerine erişmesine Izin verme</span><span class="sxs-lookup"><span data-stu-id="e3f3a-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="e3f3a-113">$false: Outlook 'ta ortak klasörlere Kullanıcı erişimini önleyin.</span><span class="sxs-lookup"><span data-stu-id="e3f3a-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="e3f3a-114">Bu, varsayılan değerdir.</span><span class="sxs-lookup"><span data-stu-id="e3f3a-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="e3f3a-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="e3f3a-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="e3f3a-116">**Not** Bu yordam yalnızca Windows için Outlook masaüstü ile bağlantıları denetleyebilir.</span><span class="sxs-lookup"><span data-stu-id="e3f3a-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="e3f3a-117">Bir Kullanıcı OWA veya Mac için Outlook kullanarak ortak klasörlere erişmeye devam edebilir.</span><span class="sxs-lookup"><span data-stu-id="e3f3a-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="e3f3a-118">Daha fazla bilgi için, [Outlook 'Ta ortak klasörlerin denetlenen bağlantıları Için destek duyurun](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="e3f3a-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>