---
title: Yedek kullanıcıyı şirket içi sunucudan silme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198584"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="0c590-102">Yedek kullanıcıyı şirket içi sunucudan silme</span><span class="sxs-lookup"><span data-stu-id="0c590-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="0c590-103">Yetim bir kullanıcıyı kaldırmak için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="0c590-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="0c590-104">[Azure Active Directory ile karma kimlik nedir?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="0c590-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="0c590-105">Dizin eşitlemesi doğrulamak için Azure [Etkin Dizini ile karma kimlik nedir?](https://technet.microsoft.com/library/jj151797.aspx)</span><span class="sxs-lookup"><span data-stu-id="0c590-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="0c590-106">Eşitleme işlevleri doğru yse, ancak Active Directory nesne silme Azure AD'ye yayınlanmiyorsa, Windows PowerShell cmdlets için aşağıdaki Azure Etkin Dizin Modülünden birini kullanarak kullanılan ürünü n</span><span class="sxs-lookup"><span data-stu-id="0c590-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="0c590-107">Kaldır-MsolContact</span><span class="sxs-lookup"><span data-stu-id="0c590-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="0c590-108">Kaldırma-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="0c590-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="0c590-109">Kaldırma-MsolUser</span><span class="sxs-lookup"><span data-stu-id="0c590-109">Remove-MsolUser</span></span>

    <span data-ttu-id="0c590-110">Örneğin, dizin eşitlemesi kullanılarak oluşturulan, ilk olarak oluşturulan kullanıcı kimliği john.smith@contoso.com kaldırmak için cmdlet'i çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="0c590-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="0c590-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="0c590-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>