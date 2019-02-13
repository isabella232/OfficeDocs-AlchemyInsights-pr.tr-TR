---
title: Profil eşitleme
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29920108"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="122f2-102">Ne zaman benim profil değişiklikleri SharePoint kullanıcı profili uygulaması için eşitleme?</span><span class="sxs-lookup"><span data-stu-id="122f2-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="122f2-103">SharePoint Çevrimiçi kullanıcılar ve gruplar kullanıcı profili uygulamasına içe aktarmak için Active Directory içe aktarma Zamanlayıcı işi (Reklam alma) kullanır.</span><span class="sxs-lookup"><span data-stu-id="122f2-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="122f2-p101">AD alma kullanıcı profili uygulaması için SharePoint çevrimiçi dizin deposu değişiklikleri eşitler. Bu değişikliklerin toplu olarak işlenir.</span><span class="sxs-lookup"><span data-stu-id="122f2-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="122f2-106">Değişiklikler eşitlenene kadar zamanlayıcı işi çalıştırır.</span><span class="sxs-lookup"><span data-stu-id="122f2-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="122f2-p102">İşi çalıştırmak için gereken süreyi işlemek için değişiklikleri sayısına bağlıdır. Çok sayıda değişiklik daha uzun sürer. Bir kullanıcı SharePoint çevrimiçi dizinde değişiklik 24 saat içinde kullanıcı profili uygulaması ' yansıtılır hizmet düzeyi sözleşmesi (SLA) belirtir.</span><span class="sxs-lookup"><span data-stu-id="122f2-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="122f2-110">SharePoint çevrimiçi kullanıcı profili eşitleme hakkında daha fazla bilgi</span><span class="sxs-lookup"><span data-stu-id="122f2-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

