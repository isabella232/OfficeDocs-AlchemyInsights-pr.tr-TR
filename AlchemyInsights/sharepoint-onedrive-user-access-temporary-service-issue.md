---
title: Performans sorunları-SharePoint veya OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719536"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="3a3a5-102">SharePoint veya OneDrive yavaş, erişilemez veya birden çok kullanıcı için kullanılamaz</span><span class="sxs-lookup"><span data-stu-id="3a3a5-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="3a3a5-103">OneDrive veya SharePoint sitesi önceden erişimi olduğu birden çok kullanıcı için kullanılabilir durumda değilse, geçici olarak hizmet sorunu olabilir.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="3a3a5-104">[Hizmet durumu panoyu kontrol edin](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="3a3a5-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="3a3a5-105">Ekleme ve kullanıcı lisansı</span><span class="sxs-lookup"><span data-stu-id="3a3a5-105">Add and license the user</span></span>

<span data-ttu-id="3a3a5-106">Emin olun, sizin [iş için Office 365'te kullanıcılara lisans atayın](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="3a3a5-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


## <a name="assign-permissions"></a><span data-ttu-id="3a3a5-107">İzinleri atama</span><span class="sxs-lookup"><span data-stu-id="3a3a5-107">Assign Permissions</span></span>

<span data-ttu-id="3a3a5-108">Kullanıcı Sharepoint lisans atadığı ve erişim engellendi iletisi almaya devam, onlar atanan [uygun izin düzeyine](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) sahip olun.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) assigned.</span></span>

## <a name="consider-using-the-access-request-feature"></a><span data-ttu-id="3a3a5-109">Erişim isteği özelliğini kullanmayı düşünün</span><span class="sxs-lookup"><span data-stu-id="3a3a5-109">Consider using the access request feature</span></span>

<span data-ttu-id="3a3a5-110">[Erişim isteği özelliği](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) şu anda görme izni olmayan içeriğe erişim isteği veriyor.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-110">The [access request feature](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

## <a name="allow-custom-script-may-cause-access-denied-issues"></a><span data-ttu-id="3a3a5-111">Özel komut dosyası erişim sorunları neden olabilir izin ver</span><span class="sxs-lookup"><span data-stu-id="3a3a5-111">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="3a3a5-112">*Özel komut dosyası izin ver* özelliği erişim engellendi burada sunmak bazı senaryolar vardır.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="3a3a5-113">Etkilenen özellikler listesi, güvenlik konuları ve özelliğini devre dışı bırakabilir.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="3a3a5-114">Lütfen ziyaret [izin ver veya özel komut dosyası engelleme](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="3a3a5-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>

