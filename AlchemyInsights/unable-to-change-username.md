---
title: Kullanıcı Adı değiştirileme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440295"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="746ae-102">Kullanıcı Adı değiştirileme</span><span class="sxs-lookup"><span data-stu-id="746ae-102">Unable to change UserName</span></span>

<span data-ttu-id="746ae-103">Bazı durumlarda, UPN (UserPrincipalName) değişiklikleri buluta yayılmaz.</span><span class="sxs-lookup"><span data-stu-id="746ae-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="746ae-104">Office 365 portalında doğrulama hataları alabilir veya kullanıcı adını veya e-posta adresini değiştiremeyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="746ae-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="746ae-105">Bu sorunu gidermek için, bu PowerShell komutunu kullanarak ManualPrincipalName'yi el ile ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="746ae-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="746ae-106">**Örnek: Kullanıcıyı yeniden adlandır**</span><span class="sxs-lookup"><span data-stu-id="746ae-106">**Example: Rename a user**</span></span>

<span data-ttu-id="746ae-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="746ae-107">PowerShellCopy</span></span>

<span data-ttu-id="746ae-108">PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="746ae-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="746ae-109">Bu komut davidc@contoso.com davidchew@contoso.com yeniden adlandırır.</span><span class="sxs-lookup"><span data-stu-id="746ae-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="746ae-110">Daha fazla bilgi için [Set-MsolUserPrincipalName'e](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0)bakın.</span><span class="sxs-lookup"><span data-stu-id="746ae-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>