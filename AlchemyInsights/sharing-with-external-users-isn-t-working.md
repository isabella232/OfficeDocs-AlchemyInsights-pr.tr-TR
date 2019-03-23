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
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 700e6d24e49cf11bf91780895f5a796cc1d8349d
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753446"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="85ab4-102">SharePoint içerik dış kullanıcılarla paylaşma sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="85ab4-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="85ab4-103">Dış paylaşımı, kuruluşunuz için açık olduğundan emin olun:</span><span class="sxs-lookup"><span data-stu-id="85ab4-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="85ab4-104">Git [Hizmetleri &amp; eklentileri Microsoft 365 Yönetim Merkezi sayfasında](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ve **Siteler**düğmesini tıklatın.</span><span class="sxs-lookup"><span data-stu-id="85ab4-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="85ab4-105">"Aç." ayarı açık olduğundan emin olun</span><span class="sxs-lookup"><span data-stu-id="85ab4-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="85ab4-106">"Varolan yalnızca dış kullanıcılar" seçilirse, harici kullanıcı Microsoft 365 Yönetim Merkezi'nde listelenen olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="85ab4-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="85ab4-107">Site için dış paylaşımı açık olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="85ab4-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="85ab4-108">Klasik site koleksiyonu için:</span><span class="sxs-lookup"><span data-stu-id="85ab4-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="85ab4-109">Sol bölmede, Klasik SharePoint Yönetim Merkezi **site koleksiyonları**' ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="85ab4-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="85ab4-110">Siteyi veya siteleri seçin ve Şerit üzerinde **Paylaşım**' ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="85ab4-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="85ab4-111">Bir Office 365 grubuna ait bir ekip sitesi veya bir iletişim sitesi için:</span><span class="sxs-lookup"><span data-stu-id="85ab4-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="85ab4-112">Kuruluş çapında ayar oturum gerektirmeyen bağlantılar kullanarak dosya paylaşımı izin vermediği sürece bu yeni site türleri aynı paylaşım kuruluş çapında ayarınız olarak ayarına sahiptir.</span><span class="sxs-lookup"><span data-stu-id="85ab4-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="85ab4-113">Bu durumda, siteler oturum yeni ve varolan dış kullanıcılar ile paylaşılmasına izin verecek.</span><span class="sxs-lookup"><span data-stu-id="85ab4-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="85ab4-114">Belirli sitelerin ayarını değiştirmek için yeni SharePoint Yönetim Merkezi (Önizleme) veya PowerShell kullanın.</span><span class="sxs-lookup"><span data-stu-id="85ab4-114">To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell.</span></span> <span data-ttu-id="85ab4-115">[Daha fazla bilgi edinin](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="85ab4-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="85ab4-116">Dış paylaşım ayarı herhangi bir site için kuruluş çapında ayarından daha fazla olmayacak izin veren ancak kuruluş çapında ayarınızı daha kısıtlayıcı olabilir.</span><span class="sxs-lookup"><span data-stu-id="85ab4-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

