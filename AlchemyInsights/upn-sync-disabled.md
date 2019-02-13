---
title: UPN eşitleme devre dışı
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 983796ce8fb7e8b52c0ce31aa13597b53cc9e038
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921728"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="04b00-102">UPN eşitleme devre dışı</span><span class="sxs-lookup"><span data-stu-id="04b00-102">UPN sync disabled</span></span>

<span data-ttu-id="04b00-103">Eşitlemeden önce 30 Mart 2016 Azure AD için başlatılan yalnızca kuruluşunuz için UPN yumuşak eşleşme sağlamak için aşağıdaki Azure AD PowerShell cmdlet'ini çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="04b00-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="04b00-104">**Kümesi-MsolDirSyncFeature-özellik EnableSoftMatchOnUpn-$True etkinleştir**</span><span class="sxs-lookup"><span data-stu-id="04b00-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="04b00-105">UPN yumuşak eşleşme Azure AD veya daha sonra 30 Mart 2016 için eşitleme başlatıldı organizasyonlar için otomatik olarak etkinleştirilir.</span><span class="sxs-lookup"><span data-stu-id="04b00-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="04b00-106">Yumuşak eşleşen UPN ve diğer eşitleme özellikleri etkinleştirme hakkında daha fazla bilgi için lütfen [Azure AD Bağlan eşitleme hizmeti özellikleri](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)bakın.</span><span class="sxs-lookup"><span data-stu-id="04b00-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

