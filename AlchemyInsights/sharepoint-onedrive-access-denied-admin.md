---
title: Erişim reddedildi iletisi ile ilgili sorunları giderme
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760360"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="badd8-102">Sharepoint/OneDrive Yönetim Merkezi erişim engellendi iletilerinde sorun giderme</span><span class="sxs-lookup"><span data-stu-id="badd8-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="badd8-103">Erişim engellendi iletisi Sharepoint/OneDrive yönetim merkezine gitmek çalışırken alıyorsanız, lütfen emin olun o [kullanıcı için bir lisans atayın](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="badd8-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="badd8-104">Kullanıcı lisansı varsa, ayrıca Yönetim Merkezleri erişebileceği [bir yönetici rolü atanmış](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) olduklarından emin olmalısınız.</span><span class="sxs-lookup"><span data-stu-id="badd8-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="badd8-105">Bu sorun, kullanıcı olduğunda ve aynı kullanıcı asıl adı ile (UPN) yeniden oluşturulması da oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="badd8-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="badd8-106">Yeni hesabı farklı bir PUID (Passport benzersiz kimliği) değeri kullanılarak oluşturulur.</span><span class="sxs-lookup"><span data-stu-id="badd8-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="badd8-107">Kullanıcı bir site koleksiyonu veya kendi OneDrive erişmeye çalıştığında, kullanıcı yanlış bir PUID sahiptir.</span><span class="sxs-lookup"><span data-stu-id="badd8-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="badd8-108">İkinci senaryo directory eşitlemesi, Active Directory kuruluş birimi (OU) ile ilgilidir.</span><span class="sxs-lookup"><span data-stu-id="badd8-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="badd8-109">Bunlar, kullanıcıların zaten SharePoint için oturumu ve ardından farklı bir kuruluş birimine taşınan ve SharePoint ile resynced, bu sorunla karşılaşabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="badd8-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="badd8-110">Bu sorunu gidermek için makaledeki adımları, [bir kullanıcının Office 365'te geri](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)ile özgün UPN kurtarmalısınız.</span><span class="sxs-lookup"><span data-stu-id="badd8-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="badd8-111">Not: bir OneDrive veya SharePoint Yönetim Merkezi önceden erişimi olduğu birden çok kullanıcı için kullanılabilir durumda değilse, bir geçici olarak hizmet sorunu olabilir.</span><span class="sxs-lookup"><span data-stu-id="badd8-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="badd8-112">[Hizmet durumu panoyu kontrol edin](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="badd8-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


