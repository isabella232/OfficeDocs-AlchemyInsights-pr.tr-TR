---
title: Exchange PowerShell ve temel kimlik doğrulamasının kullanımdan kaldırılması
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015709"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="c7e38-102">Exchange PowerShell ve temel kimlik doğrulamasının kullanımdan kaldırılması</span><span class="sxs-lookup"><span data-stu-id="c7e38-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="c7e38-103">Temel kimlik doğrulaması olmadan Exchange Online PowerShell'e bağlanma hakkında en son bilgiler için [lütfen bu sayfaya gidin](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="c7e38-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="c7e38-104">İstemci makinenizde Temel Kimlik Doğrulaması’nın yine de etkinleştirilmesi gerektiğini unutmayın.</span><span class="sxs-lookup"><span data-stu-id="c7e38-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="c7e38-105">Yeni PowerShell V2 modülü tüm REST tabanlı V2 Cmdlet’lerini etkinleştirmek için bağlantı kurarken Modern Kimlik Doğrulaması kullanır.</span><span class="sxs-lookup"><span data-stu-id="c7e38-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="c7e38-106">V2 cmdlet’lerinin yanı sıra, Uzak PowerShell oturumu kurulmasını gerektiren eski Uzak PowerShell (RPS) Cmdlet’lerine de erişmenize olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="c7e38-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="c7e38-107">Modül hizmette kimlik doğrulaması yaparken Modern Kimlik Doğrulaması mekanizmasını kullansa bile, Windows makinesinde RPS oturumu oluşturmak için istemci makinesinde WinRM Temel Kimlik Doğrulaması’nın etkinleştirilmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="c7e38-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="c7e38-108">Modern Kimlik Doğrulaması belirteçlerini aktarmak için WinRM Temel Kimlik Doğrulaması işlem hattı kullanılır.</span><span class="sxs-lookup"><span data-stu-id="c7e38-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="c7e38-109">İstemci makinesinde WinRM Temel Kimlik Doğrulaması devre dışı bırakılırsa yeni V2 cmdlet’leri çalışmaya devam eder (ama eski RPS cmdlet’leri çalışmaz).</span><span class="sxs-lookup"><span data-stu-id="c7e38-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
