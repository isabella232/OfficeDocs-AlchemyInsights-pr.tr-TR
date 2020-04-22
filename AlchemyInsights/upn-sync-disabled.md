---
title: UPN eşitleme devre dışı
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726124"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="5bb9d-102">UPN eşitleme devre dışı</span><span class="sxs-lookup"><span data-stu-id="5bb9d-102">UPN sync disabled</span></span>

<span data-ttu-id="5bb9d-103">Azure AD ile 30 Mart 2016'dan önce eşitolmaya başladıysanız, yalnızca kuruluşunuz için UPN yumuşak eşleşmesini etkinleştirmek için aşağıdaki Azure AD PowerShell cmdlet'ini çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="5bb9d-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="5bb9d-104">**Set-MsolDirSyncFeature -Özellik EnableSoftMatchOnUpn -Enable $True**</span><span class="sxs-lookup"><span data-stu-id="5bb9d-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="5bb9d-105">30 Mart 2016 tarihinde veya sonrasında Azure AD ile eşitlemeye başlayan kuruluşlar için UPN soft match otomatik olarak açılır.</span><span class="sxs-lookup"><span data-stu-id="5bb9d-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="5bb9d-106">UPN ve diğer eşitleme özelliklerinde yumuşak eşleşme sağlama hakkında daha fazla bilgi edinmek için lütfen [Azure AD Connect eşitleme hizmeti özelliklerine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)bakın.</span><span class="sxs-lookup"><span data-stu-id="5bb9d-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

