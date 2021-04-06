---
title: Windows Sanal Masaüstü sorunlarını belirleme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596037"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="f8f18-102">Windows Sanal Masaüstü sorunlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="f8f18-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="f8f18-103">Windows Sanal Masaüstü Tanılama yalnızca bir PowerShell cmdlet'i kullanır, ancak sorunları daraltmaya ve yalıtmak için isteğe bağlı birçok parametre içerir.</span><span class="sxs-lookup"><span data-stu-id="f8f18-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="f8f18-104">Başlamak için:</span><span class="sxs-lookup"><span data-stu-id="f8f18-104">To get started:</span></span> 

1. <span data-ttu-id="f8f18-105">Windows Sanal Masaüstü PowerShell modülünü indirin ve içeri aktarın.</span><span class="sxs-lookup"><span data-stu-id="f8f18-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="f8f18-106">Ayrıntılar için Windows [PowerShell için Windows Sanal Masaüstü Cmdlet'leri'ne bakın.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="f8f18-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="f8f18-107">Hesabınızla oturum açma için aşağıdaki cmdlet'i çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="f8f18-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="f8f18-108">Örnek: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="f8f18-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="f8f18-109">**NOT:** PowerShell kullanan tüm sorgular -UserName veya -ActivityID parametrelerini içermeli.</span><span class="sxs-lookup"><span data-stu-id="f8f18-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="f8f18-110">İzleme özellikleri için bkz. Tanılama [özelliği için Log Analytics kullanma.](https://go.microsoft.com/fwlink/?linkid=2126847)</span><span class="sxs-lookup"><span data-stu-id="f8f18-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="f8f18-111">Tanılama etkinliklerini kullanıcıya göre filtrelemek için, aşağıdaki cmdlet'i çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="f8f18-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="f8f18-112">Örnek: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="f8f18-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="f8f18-113">Sorunları tanılamak için çalıştırabilirsiniz filtrelerin listesi vardır.</span><span class="sxs-lookup"><span data-stu-id="f8f18-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="f8f18-114">Sorunları tanılama hakkında daha fazla bilgi edinmek için Bkz. Windows Sanal [Masaüstü sorunlarını tanımlama ve tanılama.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="f8f18-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="f8f18-115">Sık karşılaşılan hatalar hakkında daha fazla bilgi edinmek için Bkz. [Yaygın hatalar senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="f8f18-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
