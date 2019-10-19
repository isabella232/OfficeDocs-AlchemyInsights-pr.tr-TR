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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554353"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="4acc2-102">Profilim ne zaman SharePoint Kullanıcı Profili Uygulamasıile senkronize olur?</span><span class="sxs-lookup"><span data-stu-id="4acc2-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="4acc2-103">SharePoint Online, kullanıcıları ve grupları Kullanıcı Profili Uygulamasına aktarmak için Active Directory Import timer işini (AD Alma) kullanır.</span><span class="sxs-lookup"><span data-stu-id="4acc2-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="4acc2-104">AD Alma, SharePoint Online Directory Store'dan Kullanıcı Profili Uygulamasına değişiklikleri eşitler.</span><span class="sxs-lookup"><span data-stu-id="4acc2-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="4acc2-105">Bu değişiklikler toplu olarak işlenir.</span><span class="sxs-lookup"><span data-stu-id="4acc2-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="4acc2-106">Zamanlayıcı işi, değişiklikler eşitlenene kadar çalışır.</span><span class="sxs-lookup"><span data-stu-id="4acc2-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="4acc2-107">İşi çalıştırmak için aldığı süre, işlemdeki değişikliklerin sayısına bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="4acc2-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="4acc2-108">Çok sayıda değişiklik daha uzun sürer.</span><span class="sxs-lookup"><span data-stu-id="4acc2-108">A large number of changes takes longer.</span></span> <span data-ttu-id="4acc2-109">Hizmet Düzeyi Sözleşmesi (SLA), SharePoint Online Dizininde bir kullanıcıdeğişikliğinin 24 saat içinde Kullanıcı Profili Uygulamasına yansıyacağını belirtir.</span><span class="sxs-lookup"><span data-stu-id="4acc2-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="4acc2-110">SharePoint Online kullanıcı profili senkronizasyonu hakkında daha fazla bilgi</span><span class="sxs-lookup"><span data-stu-id="4acc2-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

