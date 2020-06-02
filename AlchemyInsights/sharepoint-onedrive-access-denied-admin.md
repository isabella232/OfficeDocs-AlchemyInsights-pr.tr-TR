---
title: Erişim Reddedilen iletileri sorun giderme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505399"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="06cc6-102">Sharepoint/OneDrive Yönetici Merkezi'nde Reddedilen iletilere Erişim Sorunu</span><span class="sxs-lookup"><span data-stu-id="06cc6-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="06cc6-103">Sharepoint/OneDrive Yönetici Merkezi'ne göz atlamaya çalışırken erişim reddedilen bir ileti alıyorsanız, lütfen [kullanıcıya bir lisans atadığınızdan](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)emin olun.</span><span class="sxs-lookup"><span data-stu-id="06cc6-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="06cc6-104">Kullanıcının bir lisansı varsa, yönetici merkezlerine erişebilecek [bir yönetici rolü](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) atanmış olduğundan da emin olmalısınız.</span><span class="sxs-lookup"><span data-stu-id="06cc6-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="06cc6-105">Bu sorun, bir kullanıcı silindiğinde ve aynı kullanıcı ana adı (UPN) ile yeniden oluşturulduğunda da oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="06cc6-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="06cc6-106">Yeni hesap farklı bir PUID (Passport Unique ID) değeri kullanılarak oluşturulur.</span><span class="sxs-lookup"><span data-stu-id="06cc6-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="06cc6-107">Kullanıcı bir site koleksiyonuna veya OneDrive'ına erişmeye çalıştığında, kullanıcıyanlış PUID'ye sahiptir.</span><span class="sxs-lookup"><span data-stu-id="06cc6-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="06cc6-108">İkinci bir senaryo, Etkin Dizin kuruluş birimi (OU) ile dizin eşitlemesi içerir.</span><span class="sxs-lookup"><span data-stu-id="06cc6-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="06cc6-109">Kullanıcılar Zaten SharePoint oturum açmış ve daha sonra farklı bir OU taşınır ve SharePoint ile yeniden senkronize, onlar bu sorunla karşılaşabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="06cc6-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="06cc6-110">Bu sorunu gidermek için, makalede adımları ile orijinal UPN geri yüklemeniz gerekir, [Microsoft 365 bir kullanıcı geri yükleme.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="06cc6-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="06cc6-111">Not: OneDrive veya SharePoint Yönetici merkezi daha önce erişimi olan birden çok kullanıcı tarafından kullanılamıyorsa, geçici bir hizmet sorunu olabilir.</span><span class="sxs-lookup"><span data-stu-id="06cc6-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="06cc6-112">[Hizmet durumu panosunu kontrol edin.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="06cc6-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


