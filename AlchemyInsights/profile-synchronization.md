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
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554353"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="1f4bd-102">Ne zaman benim profil değişiklikleri SharePoint kullanıcı profili uygulaması için eşitleme?</span><span class="sxs-lookup"><span data-stu-id="1f4bd-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="1f4bd-103">SharePoint Çevrimiçi kullanıcılar ve gruplar kullanıcı profili uygulamasına içe aktarmak için Active Directory içe aktarma Zamanlayıcı işi (Reklam alma) kullanır.</span><span class="sxs-lookup"><span data-stu-id="1f4bd-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="1f4bd-104">AD alma kullanıcı profili uygulaması için SharePoint çevrimiçi dizin deposu değişiklikleri eşitler.</span><span class="sxs-lookup"><span data-stu-id="1f4bd-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="1f4bd-105">Bu değişikliklerin toplu olarak işlenir.</span><span class="sxs-lookup"><span data-stu-id="1f4bd-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="1f4bd-106">Değişiklikler eşitlenene kadar zamanlayıcı işi çalıştırır.</span><span class="sxs-lookup"><span data-stu-id="1f4bd-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="1f4bd-107">İşi çalıştırmak için gereken süreyi işlemek için değişiklikleri sayısına bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="1f4bd-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="1f4bd-108">Çok sayıda değişiklik daha uzun sürer.</span><span class="sxs-lookup"><span data-stu-id="1f4bd-108">A large number of changes takes longer.</span></span> <span data-ttu-id="1f4bd-109">Bir kullanıcı SharePoint çevrimiçi dizinde değişiklik 24 saat içinde kullanıcı profili uygulaması ' yansıtılır hizmet düzeyi sözleşmesi (SLA) belirtir.</span><span class="sxs-lookup"><span data-stu-id="1f4bd-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="1f4bd-110">SharePoint çevrimiçi kullanıcı profili eşitleme hakkında daha fazla bilgi</span><span class="sxs-lookup"><span data-stu-id="1f4bd-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

