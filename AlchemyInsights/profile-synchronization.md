---
title: Profil eşitleme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801789"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="c1da9-102">Profilim SharePoint kullanıcı profili uygulamasıyla eşitlensin mi?</span><span class="sxs-lookup"><span data-stu-id="c1da9-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="c1da9-103">SharePoint Online, Kullanıcı ve grupları Kullanıcı profili uygulamasına aktarmak için Active Directory Içeri aktarma zamanlayıcı işini (AD aktarma) kullanır.</span><span class="sxs-lookup"><span data-stu-id="c1da9-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="c1da9-104">AD alma, SharePoint Online dizin deposundaki değişiklikleri Kullanıcı profili uygulamasına eşitler.</span><span class="sxs-lookup"><span data-stu-id="c1da9-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="c1da9-105">Bu değişiklikler toplu olarak işlenir.</span><span class="sxs-lookup"><span data-stu-id="c1da9-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="c1da9-106">Değişiklikler eşitlenene kadar Zamanlayıcı işi çalışır.</span><span class="sxs-lookup"><span data-stu-id="c1da9-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="c1da9-107">İşin çalışacağı süre, işlenecek değişiklik sayısına bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="c1da9-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="c1da9-108">Çok sayıda değişiklik uzun sürer.</span><span class="sxs-lookup"><span data-stu-id="c1da9-108">A large number of changes takes longer.</span></span> <span data-ttu-id="c1da9-109">Hizmet düzeyi sözleşmesi (SLA), SharePoint Online dizinindeki bir kullanıcıya yapılan değişikliğin 24 saat içinde Kullanıcı profili uygulamasına yansıtılacağını belirtir.</span><span class="sxs-lookup"><span data-stu-id="c1da9-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="c1da9-110">SharePoint Online 'da Kullanıcı profili eşitleme hakkında daha fazla bilgi</span><span class="sxs-lookup"><span data-stu-id="c1da9-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

