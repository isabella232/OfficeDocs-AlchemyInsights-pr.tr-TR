---
title: OneDrive İş Web OneDrive, Delve'e yeniden yönlendirilmesi
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51800009"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="1a779-102">OneDrive'a tık olduktan sonra Delve'e yeniden yönlendirildi</span><span class="sxs-lookup"><span data-stu-id="1a779-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="1a779-103">Ayrıntılı Sorun Giderme [Kılavuzumıza bakın.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="1a779-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="1a779-104">Bu sorunu çözmek için, yöneticinin kullanıcılara Kendi Sitelerim sitelerini oluşturma iznini vermi gerekir.</span><span class="sxs-lookup"><span data-stu-id="1a779-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="1a779-105">Bunun nedeni, OneDrive İş sayfasının Sitelerim'de oluşturulmuştur.</span><span class="sxs-lookup"><span data-stu-id="1a779-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="1a779-106">Bu hakkı vermek için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="1a779-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="1a779-107">SharePoint yönetim merkezinde kullanıcı profilleri **'ne tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="1a779-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="1a779-108">Kişiler bölümünde **Kullanıcı** İzinlerini Yönet **'e tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="1a779-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="1a779-109">Sitelerim sitesini oluşturmak için izin gerektiren kullanıcıları ekleyin.</span><span class="sxs-lookup"><span data-stu-id="1a779-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="1a779-110">Varsayılan olarak, bu ayar Dış kullanıcılar hariç **herkes olarak ayarlanır.**</span><span class="sxs-lookup"><span data-stu-id="1a779-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="1a779-111">Kullanıcı, kullanıcı veya grup ekledikten sonra eklenen kullanıcı, kullanıcı veya grubun seçili olduğundan  emin olun, izinler bölümüne ilerleyin ve Sonra Kişisel Site Oluştur (kişisel depolama alanı, haber akışı ve takip edilen içerik için **gereklidir)** öğesinin yanındaki onay kutusunu seçin.</span><span class="sxs-lookup"><span data-stu-id="1a779-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="1a779-112">**Tamam'a** tıklayın ve siteyi oluşturmak için kullanıcının OneDrive sayfasına göz attırtır.</span><span class="sxs-lookup"><span data-stu-id="1a779-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
