---
title: Dış kullanıcılarla paylaşım çalışmıyor
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691595"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="76e9a-102">Dış kullanıcılarla SharePoint içeriğini paylaşma sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="76e9a-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="76e9a-103">Kuruluşunuzda dış paylaşımın açık olduğundan emin olun:</span><span class="sxs-lookup"><span data-stu-id="76e9a-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="76e9a-104">[ &amp; Microsoft 365 Yönetim Merkezi 'nde hizmetler eklentileri sayfasına](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)gidin ve **siteler**'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="76e9a-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="76e9a-105">Ayarın "açık" olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="76e9a-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="76e9a-106">"Yalnızca mevcut dış kullanıcılar" seçiliyse, dış kullanıcının Microsoft 365 Yönetim merkezinde listelendiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="76e9a-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="76e9a-107">Site için dış paylaşımın açık olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="76e9a-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="76e9a-108">Klasik site koleksiyonu için:</span><span class="sxs-lookup"><span data-stu-id="76e9a-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="76e9a-109">Yeni SharePoint Yönetim merkezinde, sol bölmede **siteler**'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="76e9a-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="76e9a-110">Siteyi veya siteleri seçin ve şeritte **Paylaşım**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="76e9a-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="76e9a-111">Microsoft 365 grubuna veya iletişim sitesine ait bir ekip sitesi için:</span><span class="sxs-lookup"><span data-stu-id="76e9a-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="76e9a-112">Kuruluş genelindeki ayarlar, oturum açma gerektirmeyen bağlantılar kullanarak dosya paylaşmaya izin vermediği sürece, bu yeni site türlerinin kuruluş genelindeki ayarı ile aynı paylaşım ayarı vardır.</span><span class="sxs-lookup"><span data-stu-id="76e9a-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="76e9a-113">Bu durumda, siteler yeni ve oturum açan dış kullanıcılarla paylaşmaya izin verir.</span><span class="sxs-lookup"><span data-stu-id="76e9a-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="76e9a-114">Belirli sitelerin ayarını değiştirmek için yeni SharePoint Yönetim merkezini veya PowerShell 'i kullanın.</span><span class="sxs-lookup"><span data-stu-id="76e9a-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="76e9a-115">[Daha fazla bilgi edinin](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="76e9a-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="76e9a-116">Herhangi bir site için dış paylaşım ayarı, kuruluş genelindeki ayardan daha kısıtlayıcı olabilir, ancak kuruluş genelindeki ayardan daha fazla izin vermez.</span><span class="sxs-lookup"><span data-stu-id="76e9a-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

