---
title: Sorun Giderme Access, İş siteleri için OneDrive'a gönderilen iletileri reddetti
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766731"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="8f70f-102">Sorun Giderme Access, İş siteleri için OneDrive'a gönderilen iletileri reddetti</span><span class="sxs-lookup"><span data-stu-id="8f70f-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="8f70f-103">Bu sorun en sık bir kullanıcı silindiğinde ve aynı kullanıcı anaadı (UPN) ile yeniden oluşturulduğunda oluşur.</span><span class="sxs-lookup"><span data-stu-id="8f70f-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="8f70f-104">Yeni hesap farklı bir PUID (Passport Unique ID) değeri kullanılarak oluşturulur.</span><span class="sxs-lookup"><span data-stu-id="8f70f-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="8f70f-105">Kullanıcı bir site koleksiyonuna veya OneDrive'ına erişmeye çalıştığında, kullanıcıyanlış PUID'ye sahiptir.</span><span class="sxs-lookup"><span data-stu-id="8f70f-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="8f70f-106">İkinci bir senaryo, Etkin Dizin kuruluş birimi (OU) ile dizin eşitlemesi içerir.</span><span class="sxs-lookup"><span data-stu-id="8f70f-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="8f70f-107">Kullanıcılar Zaten SharePoint oturum açmış ve daha sonra farklı bir OU taşınır ve SharePoint ile yeniden senkronize, onlar bu sorunla karşılaşabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8f70f-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="8f70f-108">Bu sorunu gidermek için, özgün UPN'yi makaledeki adımlarla geri yüklemeniz gerekir, [Office 365'te bir kullanıcıyı geri yüklemelisiniz.](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="8f70f-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="8f70f-109">Orijinal kullanıcıyı geri yükleyemiyorsanız, bu adımları kullanarak eski kullanıcıyı OneDrive sitesinden kaldırmanız gerekir, [Kullanıcı bilgi listesinden bir kullanıcıyı kaldırın.]()</span><span class="sxs-lookup"><span data-stu-id="8f70f-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="8f70f-110">Bu işlem yapıldıktan sonra, kullanıcının [OneDrive'ı için yönetici ekle](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) adımlarını izleyerek kullanıcının OneDrive sitesinin yönetici haklarına sahip olduğunu doğrulayabilirsiniz</span><span class="sxs-lookup"><span data-stu-id="8f70f-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="8f70f-111">İzin düzeyleri hakkında daha fazla bilgi için, [sharepoint'teki izin düzeylerini anlama makalesine](https://docs.microsoft.com/sharepoint/understanding-permission-levels)bakın.</span><span class="sxs-lookup"><span data-stu-id="8f70f-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
