---
title: Yammer yöneticileri hakkında
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2021
ms.locfileid: "51038128"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="a9ef0-102">Yammer yöneticileri hakkında</span><span class="sxs-lookup"><span data-stu-id="a9ef0-102">About Yammer admins</span></span>

<span data-ttu-id="a9ef0-103">**Ağ yöneticileri**</span><span class="sxs-lookup"><span data-stu-id="a9ef0-103">**Network admins**</span></span>

<span data-ttu-id="a9ef0-104">Genel yöneticiler, Yammer ağı içinde otomatik olarak Doğrulanmış Yönetici rolüne yükseltilir.</span><span class="sxs-lookup"><span data-stu-id="a9ef0-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="a9ef0-105">Aşağıdaki durumlarda, bu promosyon doğru şekilde ortaya çıkar:</span><span class="sxs-lookup"><span data-stu-id="a9ef0-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="a9ef0-106">Birden çok Yammer ağı vardır ve yönetici yanlış ağda oturum açmalı.</span><span class="sxs-lookup"><span data-stu-id="a9ef0-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="a9ef0-107">[Bir Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) ağına erişim için ağ birleştirme gereklidir.</span><span class="sxs-lookup"><span data-stu-id="a9ef0-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="a9ef0-108">Azure PIM kullanılıyor.</span><span class="sxs-lookup"><span data-stu-id="a9ef0-108">Azure PIM is being used.</span></span> <span data-ttu-id="a9ef0-109">Kullanıcı, promosyonu yapmak için yeteri kadar uzun süre genel yöneticiye yükseltilemiyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="a9ef0-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="a9ef0-110">Gelecekteki bir Yammer güncelleştirmesi bu sorunu çözebilir, ancak en iyisi kullanıcıları el ile genel yöneticiye tanıtmaktır.</span><span class="sxs-lookup"><span data-stu-id="a9ef0-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="a9ef0-111">Yammer ağıyla ilgili bir eşitleme sorunu var.</span><span class="sxs-lookup"><span data-stu-id="a9ef0-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="a9ef0-112">Bu durumda, daha fazla araştırma için bir destek isteği gerekir.</span><span class="sxs-lookup"><span data-stu-id="a9ef0-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="a9ef0-113">Yammer yönetici rolleri hakkında daha fazla bilgi için Bkz. [Yammer yöneticilerini yönetme.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)</span><span class="sxs-lookup"><span data-stu-id="a9ef0-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="a9ef0-114">**Grup yöneticileri**</span><span class="sxs-lookup"><span data-stu-id="a9ef0-114">**Group admins**</span></span>

<span data-ttu-id="a9ef0-115">Microsoft 365 bağlantılı grupların grup yöneticileri, Azure AD'den grup üyeliğiyle eşitler.</span><span class="sxs-lookup"><span data-stu-id="a9ef0-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="a9ef0-116">Büyük gruplarda, bu eşitlemenin süresi uzatılabilir.</span><span class="sxs-lookup"><span data-stu-id="a9ef0-116">For large groups, this sync can take an extended period.</span></span>
