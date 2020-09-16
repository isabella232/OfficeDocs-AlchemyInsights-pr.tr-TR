---
title: Performans sorunları-SharePoint veya OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771264"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="80695-102">SharePoint veya OneDrive yavaş, birden çok kullanıcı için erişilemez veya kullanılamıyor</span><span class="sxs-lookup"><span data-stu-id="80695-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="80695-103">Bir OneDrive veya SharePoint sitesi daha önce erişimi olan birden çok kullanıcı için kullanılamıyorsa geçici bir hizmet sorunu olabilir.</span><span class="sxs-lookup"><span data-stu-id="80695-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="80695-104">[Hizmet durumu panosunu denetleyin](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="80695-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="80695-105">**Kullanıcı ekleme ve lisans**</span><span class="sxs-lookup"><span data-stu-id="80695-105">**Add and license the user**</span></span>

<span data-ttu-id="80695-106">[Microsoft 365 iş 'te kullanıcılara lisans atadığınızdan](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)emin olun.</span><span class="sxs-lookup"><span data-stu-id="80695-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="80695-107">**Izinleri atama**</span><span class="sxs-lookup"><span data-stu-id="80695-107">**Assign Permissions**</span></span>

<span data-ttu-id="80695-108">Kullanıcıya bir SharePoint lisansı atanmışsa ve erişim reddedildi iletisi almaya devam ediyorsa, lütfen [uygun izin düzeyinin uygun](https://docs.microsoft.com/sharepoint/understanding-permission-levels) olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="80695-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="80695-109">**Erişim isteği özelliğini kullanmayı düşünebilirsiniz**</span><span class="sxs-lookup"><span data-stu-id="80695-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="80695-110">[Erişim isteği özelliği](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) , kişilerin Şu anda görme izni olmayan içeriklere erişim istemesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="80695-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="80695-111">**Özel Betik**</span><span class="sxs-lookup"><span data-stu-id="80695-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="80695-112">*Özel betikte Izin ver* özelliğinin erişim reddi sunubilecekleri belirli senaryolar vardır.</span><span class="sxs-lookup"><span data-stu-id="80695-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="80695-113">Etkilenen özelliklerin listesi için güvenlik konuları ve özelliği devre dışı bırakma özelliği.</span><span class="sxs-lookup"><span data-stu-id="80695-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="80695-114">Lütfen [Izin ver veya özel betik önle](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)öğesini ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="80695-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

