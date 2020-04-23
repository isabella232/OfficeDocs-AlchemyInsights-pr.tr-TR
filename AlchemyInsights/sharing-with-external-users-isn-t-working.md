---
title: Harici kullanıcılarla paylaşmak çalışmıyor
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 285535d6144825f0935bf72579a483260c2f2bd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767269"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="268c5-102">SharePoint içeriğini dış kullanıcılarla paylaşan sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="268c5-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="268c5-103">Kuruluşunuz için dış paylaşımın açık olduğundan emin olun:</span><span class="sxs-lookup"><span data-stu-id="268c5-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="268c5-104">[Microsoft 365 &amp; yönetici merkezindeki Hizmetler eklentileri sayfasına](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)gidin ve **Siteler'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="268c5-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="268c5-105">Ayarın "Açık" olarak döndürüldiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="268c5-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="268c5-106">"Yalnızca varolan harici kullanıcılar" seçilirse, dış kullanıcının Microsoft 365 yönetici merkezinde listelenmiş olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="268c5-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="268c5-107">Site için dış paylaşımın açık olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="268c5-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="268c5-108">Klasik bir site koleksiyonu için:</span><span class="sxs-lookup"><span data-stu-id="268c5-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="268c5-109">Yeni SharePoint yönetici merkezinde, sol **bölmede, siteleri**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="268c5-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="268c5-110">Siteyi veya siteleri seçin ve şeritte **Paylaşım'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="268c5-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="268c5-111">Office 365 grubuna veya bir iletişim sitesine ait bir ekip sitesi için:</span><span class="sxs-lookup"><span data-stu-id="268c5-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="268c5-112">Kuruluş genelinde ayar oturum açma gerektirmeyen bağlantıları kullanarak dosyaların paylaşılmasına izin vermese, bu yeni site türleri kuruluş genelindeki ayarınızla aynı paylaşım ayarına sahiptir.</span><span class="sxs-lookup"><span data-stu-id="268c5-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="268c5-113">Bu durumda, siteler oturum kuran yeni ve varolan harici kullanıcılarla paylaşıma izin verir.</span><span class="sxs-lookup"><span data-stu-id="268c5-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="268c5-114">Belirli sitelerin ayarını değiştirmek için yeni SharePoint yönetici merkezini veya PowerShell'i kullanın.</span><span class="sxs-lookup"><span data-stu-id="268c5-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="268c5-115">[Daha fazla bilgi edinin](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="268c5-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="268c5-116">Herhangi bir sitenin dış paylaşım ayarı kuruluş çapındaki ayarınızdan daha kısıtlayıcı olabilir, ancak kuruluş genelindeki ayarından daha izin verilebilir.</span><span class="sxs-lookup"><span data-stu-id="268c5-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

