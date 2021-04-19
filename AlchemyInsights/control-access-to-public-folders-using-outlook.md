---
title: Outlook'u kullanarak ortak klasörlere erişimi denetleme
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816760"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="2c7e3-102">Outlook'u kullanarak ortak klasörlere erişimi denetleme</span><span class="sxs-lookup"><span data-stu-id="2c7e3-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="2c7e3-103">Outlook'u kullanarak ortak klasörlere hangi kullanıcıların eriş erişeni kontrol etmek için:</span><span class="sxs-lookup"><span data-stu-id="2c7e3-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="2c7e3-104">Kullanım `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="2c7e3-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="2c7e3-105">$true: Kullanıcıların Outlook'ta ortak klasörlere erişmesine izin verme</span><span class="sxs-lookup"><span data-stu-id="2c7e3-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="2c7e3-106">$false: Outlook'ta kullanıcının ortak klasörlere erişimini engelin.</span><span class="sxs-lookup"><span data-stu-id="2c7e3-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="2c7e3-107">Bu, varsayılan değerdir.</span><span class="sxs-lookup"><span data-stu-id="2c7e3-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="2c7e3-108">Not: Bu yordam yalnızca Windows istemcileri için Outlook masaüstü ile bağlantıları kontrol eder.</span><span class="sxs-lookup"><span data-stu-id="2c7e3-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="2c7e3-109">Kullanıcılar ortak klasörlere OWA veya Mac için Outlook'u kullanarak erişmeye devam ediyor.</span><span class="sxs-lookup"><span data-stu-id="2c7e3-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="2c7e3-110">Daha fazla bilgi için bkz. [Outlook'ta Ortak Klasörlere Denetimli](https://aka.ms/controlpf) Bağlantılar.</span><span class="sxs-lookup"><span data-stu-id="2c7e3-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
