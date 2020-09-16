---
title: UPN eşitlemesi devre dışı bırakıldı
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749534"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="b2f20-102">UPN eşitlemesi devre dışı bırakıldı</span><span class="sxs-lookup"><span data-stu-id="b2f20-102">UPN sync disabled</span></span>

<span data-ttu-id="b2f20-103">30 Mart 2016 tarihinden önce Azure AD ile eşitleme işlemini başlattıysanız, yalnızca kuruluşunuzda UPN kolay eşleşmesinden etkinleştirmek için aşağıdaki Azure AD PowerShell cmdlet 'ini çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="b2f20-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="b2f20-104">**Set-MsolDirSyncFeature-Feature Enablesoftmatch, UPN-Enable $True**</span><span class="sxs-lookup"><span data-stu-id="b2f20-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="b2f20-105">%30 Mart 2016 tarihinde veya sonrasında Azure AD 'e eşitlemeyi Başlatan kuruluşlar için UPN yazılımdan eşleşme otomatik olarak açıktır.</span><span class="sxs-lookup"><span data-stu-id="b2f20-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="b2f20-106">UPN ve diğer eşitleme özelliklerinde yazılımla eşleştirmeyi etkinleştirme hakkında daha fazla bilgi edinmek için lütfen [Azure AD Connect eşitleme hizmeti özelliklerine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)bakın.</span><span class="sxs-lookup"><span data-stu-id="b2f20-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

