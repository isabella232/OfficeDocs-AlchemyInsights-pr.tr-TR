---
title: MSCommerce modülüne bağlanın
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 10ef2e8fa7c564d53177a52136eb48cd709e5c55
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158535"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="44a19-102">MSCommerce bir Şirket veya Fatura Yöneticisi hesabı gerektirir</span><span class="sxs-lookup"><span data-stu-id="44a19-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="44a19-103">MSCommerce modülü, Şirket veya Fatura Yöneticisi ayrıcalıklarına sahip bir hesap gerektirir.</span><span class="sxs-lookup"><span data-stu-id="44a19-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="44a19-104">Aşağıdaki hatayı alıyorsanız, farklı bir hesapla yeniden bağlanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="44a19-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

<span data-ttu-id="44a19-105">*ErrorMessage - Uzak sunucu bir hata döndü: (403) Yasak. HataAyrıntıları - C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span><span class="sxs-lookup"><span data-stu-id="44a19-105">*ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span></span><br>
<span data-ttu-id="44a19-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Alınamadı ...*</span><span class="sxs-lookup"><span data-stu-id="44a19-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span></span><br>
<span data-ttu-id="44a19-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span><span class="sxs-lookup"><span data-stu-id="44a19-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span></span><br>
<span data-ttu-id="44a19-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : Belirtilmedi: (:) [Yazma-Hata], WriteErrorException*</span><span class="sxs-lookup"><span data-stu-id="44a19-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException*</span></span><br>
<span data-ttu-id="44a19-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ Tam NitelikliErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span><span class="sxs-lookup"><span data-stu-id="44a19-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span></span>

<span data-ttu-id="44a19-110">Hesabınızda Şirket veya Fatura Yöneticisi ayrıcalıkları yoksa BT Yöneticinize başvurun.</span><span class="sxs-lookup"><span data-stu-id="44a19-110">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
