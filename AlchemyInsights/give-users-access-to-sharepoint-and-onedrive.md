---
title: Kullanıcılara SharePoint ve OneDrive 'a erişim verme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677227"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="87669-102">Kullanıcılara SharePoint ve OneDrive 'a erişim verme</span><span class="sxs-lookup"><span data-stu-id="87669-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="87669-103">Bir OneDrive veya SharePoint sitesi daha önce erişimi olan birden çok kullanıcı için kullanılamıyorsa geçici bir hizmet sorunu olabilir.</span><span class="sxs-lookup"><span data-stu-id="87669-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="87669-104">Hizmet durumu panosunu denetleme</span><span class="sxs-lookup"><span data-stu-id="87669-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="87669-105">Kuruluşunuzdaki kişilerin SharePoint ve OneDrive 'ı kullanmasını istiyorsanız, onlara hesap eklemeniz ve SharePoint ve OneDrive 'a erişim sağlayan bir lisansı olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="87669-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="87669-106">Kullanıcıları eklemenin en kolay yolu Microsoft 365 Yönetim merkezindedir.</span><span class="sxs-lookup"><span data-stu-id="87669-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="87669-107">[Microsoft 365 Yönetim Merkezi 'Nde etkin kullanıcılar sayfasına](https://portal.office.com/adminportal/home#/users)gidin ve ardından **Kullanıcı Ekle**'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="87669-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="87669-108">Kullanıcının bilgilerini doldurun ve **ürün lisanslarının**altında, lisans atanmış ve **SharePoint Online** 'ın seçili olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="87669-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="87669-109">Kuruluşunuzda dış paylaşıma izin verirseniz, kullanıcıların kuruluş dışından kişilerle SharePoint ve OneDrive içeriğini paylaşabileceği dikkate alın.</span><span class="sxs-lookup"><span data-stu-id="87669-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="87669-110">Bu dış kullanıcı lisanslarını vermeniz gerekmez.</span><span class="sxs-lookup"><span data-stu-id="87669-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="87669-111">Paylaşım "yalnızca var olan dış kullanıcılar" olarak ayarlanmadıkça de onlara hesap eklemeniz gerekmez.</span><span class="sxs-lookup"><span data-stu-id="87669-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="87669-112">Bu durumda, insanlar kuruluşunuzun dizininde değillerse, bunları Azure AD Yönetim Merkezi 'nde Konuk Kullanıcı olarak eklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="87669-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

