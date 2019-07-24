---
title: SharePoint veya OneDrive kullanmaya çalışırken bakım ileti için salt okunur
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: cc232fba6f502e2b6f282a8c1a1e29221e36b70d
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840535"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="fd1ec-102">SharePoint veya OneDrive kullanmaya çalışırken bakım ileti için salt okunur</span><span class="sxs-lookup"><span data-stu-id="fd1ec-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="fd1ec-103">Kullanıcılar, SharePoint veya OneDrive kullanmaya çalışırken bir **Bakım için salt okunur** ileti alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fd1ec-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive.</span></span>  <span data-ttu-id="fd1ec-104">Bu durumda, [İleti Merkezi](https://portal.office.com/adminportal/home#/MessageCenter)giderek, Kiracı üzerinde gerçekleşen etkin bakım olup olmadığını denetleyin.</span><span class="sxs-lookup"><span data-stu-id="fd1ec-104">If so, check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span> <span data-ttu-id="fd1ec-105">Ayrıca, herhangi danışma /, oluşabilecek KAZALARI için denetlemek için [Sağlık Hizmeti](https://portal.office.com/adminportal/home#/servicehealth) panoyu kontrol ettiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="fd1ec-105">Also, make sure to check the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) dashboard to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="fd1ec-106">Pano ne ileti merkezi ya da Sağlık Hizmeti geçerli bakımı hakkında hiçbir şey, Kiracı için dikkate aldıysanız, bu sorunu önbelleğe tarayıcı olabilir.</span><span class="sxs-lookup"><span data-stu-id="fd1ec-106">If neither the Message Center or Service Health dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="fd1ec-107">Lütfen siteye gitmeden önce tarayıcı önbelleği temizlemek deneyin.</span><span class="sxs-lookup"><span data-stu-id="fd1ec-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="fd1ec-108">Microsoft Edge tarayıcınızın **ayarlarını**seçin ve ardından **Gizlilik ve güvenlik**seçin.</span><span class="sxs-lookup"><span data-stu-id="fd1ec-108">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="fd1ec-109">**Clear göz**altında **temizlemek ne seçin**seçin.</span><span class="sxs-lookup"><span data-stu-id="fd1ec-109">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="fd1ec-110">**Tanımlama bilgileri ve kaydedilmiş Web sitesi verilerini**seçin ve **Temizle'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="fd1ec-110">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="fd1ec-111">Bu adımlar, Mozilla Firefox veya Google Chrome gibi başka tarayıcıları kullanırken, farklı olabilir.</span><span class="sxs-lookup"><span data-stu-id="fd1ec-111">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="fd1ec-112">SharePoint sitesi veya OneDrive yeni InPrivate penceresinde açmak için başka bir seçenek olacaktır.</span><span class="sxs-lookup"><span data-stu-id="fd1ec-112">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>