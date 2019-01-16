---
title: UPN eşitleme devre dışı
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28318494"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="da072-102">UPN eşitleme devre dışı</span><span class="sxs-lookup"><span data-stu-id="da072-102">UPN sync disabled</span></span>

<span data-ttu-id="da072-103">Eşitlemeden önce 30 Mart 2016 Azure AD için başlatılan yalnızca kuruluşunuz için UPN yumuşak eşleşme sağlamak için aşağıdaki Azure AD PowerShell cmdlet'ini çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="da072-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="da072-104">**Kümesi-MsolDirSyncFeature-özellik EnableSoftMatchOnUpn-$True etkinleştir**</span><span class="sxs-lookup"><span data-stu-id="da072-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="da072-105">UPN yumuşak eşleşme Azure AD veya daha sonra 30 Mart 2016 için eşitleme başlatıldı organizasyonlar için otomatik olarak etkinleştirilir.</span><span class="sxs-lookup"><span data-stu-id="da072-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="da072-106">Yumuşak eşleşen UPN ve diğer eşitleme özellikleri etkinleştirme hakkında daha fazla bilgi için lütfen [Azure AD Bağlan eşitleme hizmeti özellikleri](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)bakın.</span><span class="sxs-lookup"><span data-stu-id="da072-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

