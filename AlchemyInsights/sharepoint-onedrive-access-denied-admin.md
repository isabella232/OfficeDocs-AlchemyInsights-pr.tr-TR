---
title: Erişim reddedildi iletilerinde sorun giderme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767683"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="5567d-102">SharePoint/OneDrive Yönetim merkezinde erişim reddedildi iletilerinde sorun giderme</span><span class="sxs-lookup"><span data-stu-id="5567d-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="5567d-103">SharePoint/OneDrive yönetim merkezine gözatmaya çalışırken erişim reddedildi iletisi alıyorsanız, lütfen [kullanıcıya lisans atadığınızdan](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)emin olun.</span><span class="sxs-lookup"><span data-stu-id="5567d-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="5567d-104">Kullanıcının lisansı varsa, bunların yönetim merkezlerine erişebilen [bir yönetici rolü atadıklarını](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) da unutmayın.</span><span class="sxs-lookup"><span data-stu-id="5567d-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="5567d-105">Bu sorun, bir Kullanıcı silindiğinde ve aynı kullanıcı asıl adıyla (UPN) yeniden oluşturulduğunda da oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="5567d-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="5567d-106">Yeni hesap farklı bir PUıD (Passport benzersiz KIMLIĞI) değeri kullanılarak oluşturulur.</span><span class="sxs-lookup"><span data-stu-id="5567d-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="5567d-107">Kullanıcı bir site koleksiyonuna veya OneDrive 'a erişmeyi denediğinde, kullanıcının yanlış PUıD 'si vardır.</span><span class="sxs-lookup"><span data-stu-id="5567d-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="5567d-108">İkinci senaryo, Active Directory kuruluş birimi (OU) ile dizin eşitlemesi içerir.</span><span class="sxs-lookup"><span data-stu-id="5567d-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="5567d-109">Kullanıcılar zaten SharePoint 'te oturumlarsa, başka bir kuruluş birimine taşınmış ve SharePoint ile yeniden eşitleniyor</span><span class="sxs-lookup"><span data-stu-id="5567d-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="5567d-110">Bu sorunu çözmek için, özgün UPN 'yi makaledeki adımlarla geri yüklemelisiniz, [Microsoft 365 'da bir kullanıcıyı geri yüklemelisiniz](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="5567d-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="5567d-111">Not: OneDrive veya SharePoint Yönetim Merkezi daha önce erişimi olan birden çok kullanıcı için kullanılamıyorsa geçici bir hizmet sorunu olabilir.</span><span class="sxs-lookup"><span data-stu-id="5567d-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="5567d-112">[Hizmet durumu panosunu denetleyin](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="5567d-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


