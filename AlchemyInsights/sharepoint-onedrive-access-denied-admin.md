---
title: Erişim Reddedildi ileti sorunlarını giderme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707974"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="b40f6-102">SharePoint/OneDrive Yönetim Merkezi'nde Erişim Reddedildi iletileriyle ilgili sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="b40f6-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="b40f6-103">SharePoint/OneDrive Yönetim Merkezi'ne göz atamazken erişim reddedildi iletisi alıyorsanız, kullanıcıya lisans [atayın.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="b40f6-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="b40f6-104">Kullanıcının lisansı varsa, bu kullanıcıya yönetim merkezlerine erişen bir [yönetici](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) rolü atanmalı.</span><span class="sxs-lookup"><span data-stu-id="b40f6-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="b40f6-105">Bu sorun, kullanıcı silindiğinde ve aynı kullanıcı asıl adıyla (UPN) yeniden oluşturulduğunda de oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="b40f6-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="b40f6-106">Yeni hesap, farklı bir PUID (Passport Benzersiz Kimlik) değeri kullanılarak oluşturulur.</span><span class="sxs-lookup"><span data-stu-id="b40f6-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="b40f6-107">Kullanıcı bir site koleksiyonuna veya OneDrive'larına erişmeye çalıştığında, kullanıcının puid'i yanlış olur.</span><span class="sxs-lookup"><span data-stu-id="b40f6-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="b40f6-108">İkinci senaryo, Active Directory kuruluş birimiyle (OU) dizin eşitlemesi içerir.</span><span class="sxs-lookup"><span data-stu-id="b40f6-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="b40f6-109">Kullanıcılar daha önce SharePoint'te oturum açmışsa ve sonra başka bir OU'ya taşınmışsa ve SharePoint ile yeniden eşitlirse, bu sorunla sınmış olabilir.</span><span class="sxs-lookup"><span data-stu-id="b40f6-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="b40f6-110">Bu sorunu çözmek için, [microsoft 365'te](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)bir kullanıcıyı geri yükleme makalesinde verilen adımları kullanarak özgün UPN'yi geri yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b40f6-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="b40f6-111">Not: OneDrive veya SharePoint Yönetim merkezi daha önce erişimi olan birden çok kullanıcı tarafından kullanılamıyorsa, geçici bir hizmet sorunu olabilir.</span><span class="sxs-lookup"><span data-stu-id="b40f6-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="b40f6-112">[Hizmet durumu panosuna göz ekleyin.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="b40f6-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


