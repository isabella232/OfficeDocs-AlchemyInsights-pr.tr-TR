---
title: MSCommerce modülüne bağlanma
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
- "9001212"
- "3529"
ms.openlocfilehash: 15dc7038426a8d436c236a91aa0f3462f6a3e366
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702635"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="a8847-102">MSCommerce şirket veya faturalandırma Yöneticisi hesabı gerektirir</span><span class="sxs-lookup"><span data-stu-id="a8847-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="a8847-103">MSCommerce modülü şirket veya faturalandırma Yöneticisi ayrıcalıklarına sahip bir hesap gerektirir.</span><span class="sxs-lookup"><span data-stu-id="a8847-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="a8847-104">Aşağıdaki hatayı alıyorsanız, başka bir hesapla yeniden bağlanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="a8847-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

<span data-ttu-id="a8847-105">*ErrorMessage-uzak sunucu hata döndürdü: (403) yasak. ErrorDetails-C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 karakter: 5*</span><span class="sxs-lookup"><span data-stu-id="a8847-105">*ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span></span><br>
<span data-ttu-id="a8847-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError-ErrorContext $ _-CustomErrorMessage "yeniden üçe geçirilemedi...*</span><span class="sxs-lookup"><span data-stu-id="a8847-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span></span><br>
<span data-ttu-id="a8847-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span><span class="sxs-lookup"><span data-stu-id="a8847-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span></span><br>
<span data-ttu-id="a8847-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo: Notbelirtildi: (:) [Write-Error], WriteErrorException*</span><span class="sxs-lookup"><span data-stu-id="a8847-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException*</span></span><br>
<span data-ttu-id="a8847-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId: Microsoft. PowerShell. Commands. WriteErrorException, HandleError*</span><span class="sxs-lookup"><span data-stu-id="a8847-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span></span>

<span data-ttu-id="a8847-110">Hesabınızda şirket veya faturalandırma Yöneticisi ayrıcalıkları yoksa BT yöneticinize başvurun.</span><span class="sxs-lookup"><span data-stu-id="a8847-110">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
