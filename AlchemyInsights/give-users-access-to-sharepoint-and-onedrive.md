---
title: Kullanıcılara SharePoint ve OneDrive'a erişim izni verin
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 0bdc2fa97ad1fe8b3280411babaaf2bd685a644d
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43721851"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="1c9f0-102">Kullanıcılara SharePoint ve OneDrive'a erişim izni verin</span><span class="sxs-lookup"><span data-stu-id="1c9f0-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="1c9f0-103">OneDrive veya SharePoint sitesi daha önce erişimi olan birden çok kullanıcı tarafından kullanılamıyorsa, geçici bir hizmet sorunu olabilir.</span><span class="sxs-lookup"><span data-stu-id="1c9f0-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="1c9f0-104">Hizmet durumu panosunu kontrol edin</span><span class="sxs-lookup"><span data-stu-id="1c9f0-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="1c9f0-105">Kuruluşunuzdaki kişilerin SharePoint ve OneDrive'da oturum açabilmesini ve bunları kullanabilmesini istiyorsanız, onlar için hesap eklemeniz ve sharepoint ve OneDrive'a erişim sağlayan bir lisansa sahip olmalarını sağlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="1c9f0-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="1c9f0-106">Kullanıcı eklemenin en kolay yolu Microsoft 365 yönetici merkezidir.</span><span class="sxs-lookup"><span data-stu-id="1c9f0-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="1c9f0-107">[Microsoft 365 yönetici merkezindeki Etkin kullanıcılar sayfasına](https://portal.office.com/adminportal/home#/users)gidin ve ardından **kullanıcı ekle'yi**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="1c9f0-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="1c9f0-108">Kullanıcının bilgilerini doldurun ve **Ürün lisansları**altında bir lisans ın atandığından ve **SharePoint Online'ın** seçildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="1c9f0-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="1c9f0-109">Kuruluşunuzda dış paylaşıma izin verirseniz, kullanıcıların SharePoint ve OneDrive içeriğini kuruluş dışındaki kişilerle paylaşabileceğini unutmayın.</span><span class="sxs-lookup"><span data-stu-id="1c9f0-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="1c9f0-110">Bu harici kullanıcılara lisans vermeniz gerekmez.</span><span class="sxs-lookup"><span data-stu-id="1c9f0-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="1c9f0-111">Paylaşım "Yalnızca varolan harici kullanıcılar" olarak ayarlmadığı sürece, onlar için hesap eklemeniz de gerekmez.</span><span class="sxs-lookup"><span data-stu-id="1c9f0-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="1c9f0-112">Bu durumda, kişiler kuruluşunuzun dizininde değilse, bunları Azure AD yönetici merkezine konuk kullanıcı olarak eklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="1c9f0-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

