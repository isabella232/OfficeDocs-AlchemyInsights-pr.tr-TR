---
title: Exchange PowerShell ve temel kimlik doğrulamasının kullanımdan kaldırılması
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
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813492"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="b6009-102">Exchange PowerShell ve temel kimlik doğrulamasının kullanımdan kaldırılması</span><span class="sxs-lookup"><span data-stu-id="b6009-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="b6009-103">Temel kimlik doğrulaması olmadan Exchange Online PowerShell'e bağlanma hakkında en son bilgiler için [lütfen bu sayfaya gidin](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="b6009-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="b6009-104">PowerShell V2 modülü temel kimlik doğrulamasını kullanmaz.</span><span class="sxs-lookup"><span data-stu-id="b6009-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="b6009-105">İstemci makinenizde Temel Kimlik Doğrulaması’nın yine de etkinleştirilmesi gerektiğini unutmayın.</span><span class="sxs-lookup"><span data-stu-id="b6009-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="b6009-106">Yeni PowerShell V2 modülü tüm REST tabanlı V2 Cmdlet’lerini etkinleştirmek için bağlantı kurarken Modern Kimlik Doğrulaması kullanır.</span><span class="sxs-lookup"><span data-stu-id="b6009-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="b6009-107">V2 cmdlet’lerinin yanı sıra, Uzak PowerShell oturumu kurulmasını gerektiren eski Uzak PowerShell (RPS) Cmdlet’lerine de erişmenize olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="b6009-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="b6009-108">Modül hizmette kimlik doğrulaması yaparken Modern Kimlik Doğrulaması mekanizmasını kullansa bile, Windows makinesinde RPS oturumu oluşturmak için istemci makinesinde WinRM Temel Kimlik Doğrulaması’nın etkinleştirilmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="b6009-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="b6009-109">Modern Kimlik Doğrulaması belirteçlerini aktarmak için WinRM Temel Kimlik Doğrulaması işlem hattı kullanılır.</span><span class="sxs-lookup"><span data-stu-id="b6009-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="b6009-110">İstemci makinesinde WinRM Temel Kimlik Doğrulaması devre dışı bırakılırsa yeni V2 cmdlet’leri çalışmaya devam eder (ama eski RPS cmdlet’leri çalışmaz).</span><span class="sxs-lookup"><span data-stu-id="b6009-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
