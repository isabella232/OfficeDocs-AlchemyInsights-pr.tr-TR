---
title: Performans sorunları-SharePoint veya OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 7e218cfff81274cd16d55dec2c5243eb8b74a3b7
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750576"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="4a6d7-102">SharePoint veya OneDrive Birden Çok Kullanıcı için Yavaş, Erişilemez veya Kullanılamıyor</span><span class="sxs-lookup"><span data-stu-id="4a6d7-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="4a6d7-103">OneDrive veya SharePoint sitesi daha önce erişimi olan birden çok kullanıcı tarafından kullanılamıyorsa, geçici bir hizmet sorunu olabilir.</span><span class="sxs-lookup"><span data-stu-id="4a6d7-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="4a6d7-104">[Hizmet durumu panosunu kontrol edin.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="4a6d7-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="4a6d7-105">**Kullanıcıyı ekleme ve lisansla**</span><span class="sxs-lookup"><span data-stu-id="4a6d7-105">**Add and license the user**</span></span>

<span data-ttu-id="4a6d7-106">[İşletmeler için Office 365'teki kullanıcılara lisans atadığınızdan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)emin olun.</span><span class="sxs-lookup"><span data-stu-id="4a6d7-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="4a6d7-107">**İzinatama**</span><span class="sxs-lookup"><span data-stu-id="4a6d7-107">**Assign Permissions**</span></span>

<span data-ttu-id="4a6d7-108">Kullanıcıya Sharepoint lisansı atanmışsa ve hala erişim reddedilen bir ileti alıyorsa, lütfen [uygun izin düzeyinin](https://docs.microsoft.com/sharepoint/understanding-permission-levels) atandığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="4a6d7-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="4a6d7-109">**Erişim isteği özelliğini kullanmayı düşünün**</span><span class="sxs-lookup"><span data-stu-id="4a6d7-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="4a6d7-110">[Erişim isteği özelliği,](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) kullanıcıların şu anda görme izni olmayan içeriğe erişim isteğinde bulunmalarına olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="4a6d7-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="4a6d7-111">**Özel komut dosyasına izin ver, erişim engellenen sorunlara neden olabilir**</span><span class="sxs-lookup"><span data-stu-id="4a6d7-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="4a6d7-112">*Özel komut dosyasına İzin Ver* özelliğinin reddedilen bir erişim sunabileceği belirli senaryolar vardır.</span><span class="sxs-lookup"><span data-stu-id="4a6d7-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="4a6d7-113">Etkilenen özelliklerin listesi, güvenlik hususları ve özelliği devre dışı bırakmak için yeteneği için.</span><span class="sxs-lookup"><span data-stu-id="4a6d7-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="4a6d7-114">Lütfen [Özel komut dosyasına İzin Ver'i ziyaret edin veya engelleyin.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="4a6d7-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

