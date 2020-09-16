---
title: OneDrive Iş Web OneDrive 'ı Delve 'e yönlendirir
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776400"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="a3954-102">OneDrive 'a tıkladıktan sonra Delve 'e yeniden yönlendiriliyor</span><span class="sxs-lookup"><span data-stu-id="a3954-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="a3954-103">Ayrıntılı [sorun giderme kılavuzuna](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)bakın.</span><span class="sxs-lookup"><span data-stu-id="a3954-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="a3954-104">Bu sorunu çözmek için yöneticinin kullanıcılara Sitelerim sitesini oluşturma hakkını vermesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="a3954-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="a3954-105">Bunun nedeni, Siteimde OneDrive Iş sayfasının oluşturulmuştu.</span><span class="sxs-lookup"><span data-stu-id="a3954-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="a3954-106">Bu hakkı vermek için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="a3954-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="a3954-107">SharePoint Yönetim merkezinde **Kullanıcı profilleri**'ne tıklayın.</span><span class="sxs-lookup"><span data-stu-id="a3954-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="a3954-108">**İnsanlar** bölümünde **Kullanıcı izinlerini Yönet**'i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="a3954-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="a3954-109">Sitelerim sitesini oluşturmak için izin gerektiren kullanıcılar ekleyin.</span><span class="sxs-lookup"><span data-stu-id="a3954-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="a3954-110">Varsayılan olarak, bu ayar **Dış Kullanıcı dışında herkes**olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="a3954-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="a3954-111">Kullanıcıyı, kullanıcıları veya grubu ekledikten sonra, eklenen Kullanıcı, kullanıcılar veya grup 'in seçili olduğundan emin olun, **izinler** bölümüne gidin ve **kişisel site oluştur (kişisel depolama, haber akışı ve takip edilen içerik için gereklidir)** yanındaki denetim kutusunu seçin.</span><span class="sxs-lookup"><span data-stu-id="a3954-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="a3954-112">**Tamam**'a tıklayın ve ardından Kullanıcı siteyi oluşturmak için OneDrive sayfasına göz atın.</span><span class="sxs-lookup"><span data-stu-id="a3954-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
