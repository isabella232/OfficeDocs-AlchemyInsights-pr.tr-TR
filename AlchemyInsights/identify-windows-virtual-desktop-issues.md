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
# <a name="identify-windows-virtual-desktop-issues"></a>Windows Sanal Masaüstü sorunlarını belirleme

Windows Sanal Masaüstü Tanılama yalnızca bir PowerShell cmdlet'i kullanır, ancak sorunları daraltmaya ve yalıtmak için isteğe bağlı birçok parametre içerir. Başlamak için: 

1. Windows Sanal Masaüstü PowerShell modülünü indirin ve içeri aktarın. Ayrıntılar için Windows [PowerShell için Windows Sanal Masaüstü Cmdlet'leri'ne bakın.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Hesabınızla oturum açma için aşağıdaki cmdlet'i çalıştırın:
    
    Örnek: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**NOT:** PowerShell kullanan tüm sorgular -UserName veya -ActivityID parametrelerini içermeli. İzleme özellikleri için bkz. Tanılama [özelliği için Log Analytics kullanma.](https://go.microsoft.com/fwlink/?linkid=2126847)

Tanılama etkinliklerini kullanıcıya göre filtrelemek için, aşağıdaki cmdlet'i çalıştırın:

Örnek: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Sorunları tanılamak için çalıştırabilirsiniz filtrelerin listesi vardır. Sorunları tanılama hakkında daha fazla bilgi edinmek için Bkz. Windows Sanal [Masaüstü sorunlarını tanımlama ve tanılama.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Sık karşılaşılan hatalar hakkında daha fazla bilgi edinmek için Bkz. [Yaygın hatalar senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
