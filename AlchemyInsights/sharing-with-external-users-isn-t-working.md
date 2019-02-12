---
title: Dış kullanıcılarla paylaşma çalışmıyor
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 20b538846997c021b6e88596a1e8aff401ea935b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900912"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="435b6-102">SharePoint içerik dış kullanıcılarla paylaşma sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="435b6-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="435b6-103">Dış paylaşımı, kuruluşunuz için açık olduğundan emin olun:</span><span class="sxs-lookup"><span data-stu-id="435b6-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="435b6-104">Git [Hizmetleri &amp; Eklentileri Office 365 Yönetim Merkezi sayfasında](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ve **Siteler**düğmesini tıklatın.</span><span class="sxs-lookup"><span data-stu-id="435b6-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="435b6-p101">"Aç." ayarı açık olduğundan emin olun "Varolan yalnızca dış kullanıcılar" seçilirse, dış kullanıcının Office 365 Yönetim Merkezi'nde listelenen olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="435b6-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="435b6-p102">Site için dış paylaşımı açık olduğundan emin olun. Klasik site koleksiyonu için:</span><span class="sxs-lookup"><span data-stu-id="435b6-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="435b6-109">Sol bölmede, Klasik SharePoint Yönetim Merkezi **site koleksiyonları**' ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="435b6-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="435b6-110">Siteyi veya siteleri seçin ve Şerit üzerinde **Paylaşım**' ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="435b6-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="435b6-111">Bir Office 365 grubuna ait bir ekip sitesi veya bir iletişim sitesi için:</span><span class="sxs-lookup"><span data-stu-id="435b6-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="435b6-p103">Kuruluş çapında ayar oturum gerektirmeyen bağlantılar kullanarak dosya paylaşımı izin vermediği sürece bu yeni site türleri aynı paylaşım kuruluş çapında ayarınız olarak ayarına sahiptir. Bu durumda, siteler oturum yeni ve varolan dış kullanıcılar ile paylaşılmasına izin verecek. Belirli sitelerin ayarını değiştirmek için yeni SharePoint Yönetim Merkezi (Önizleme) veya PowerShell kullanın. [Daha fazla bilgi edinin](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="435b6-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="435b6-116">Dış paylaşım ayarı herhangi bir site için kuruluş çapında ayarından daha fazla olmayacak izin veren ancak kuruluş çapında ayarınızı daha kısıtlayıcı olabilir.</span><span class="sxs-lookup"><span data-stu-id="435b6-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

