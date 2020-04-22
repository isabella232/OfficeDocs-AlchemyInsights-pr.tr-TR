---
title: Ediscovery dışa aktarma için Krom tarayıcılarına dayalı Microsoft Edge'i kullanma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: 5c247ab69c272d2d296f9602fc5246a08164da5e
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726232"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="26b91-102">Ediscovery dışa aktarma için Krom tarayıcılarına dayalı Microsoft Edge'i kullanma</span><span class="sxs-lookup"><span data-stu-id="26b91-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="26b91-103">Son değişiklik nedeniyle, Microsoft Edge tarayıcılarında artık varsayılan olarak ClickOnce desteği etkinleştirilen olmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="26b91-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="26b91-104">Microsoft 365 eDiscovery Dışa Aktarma Aracı'nı kullanmaya devam etmek için Microsoft Internet Explorer'ı kullanmanız veya Microsoft Edge'de ClickOnce Desteği'ni etkinleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="26b91-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="26b91-105">Chromium'a dayalı olarak Microsoft Edge'de ClickOnce Desteği'ni etkinleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="26b91-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="26b91-106">Microsoft Edge tarayıcınızda edge://flags/#edge-click-once'yi ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="26b91-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="26b91-107">ClickOnce Desteği seçeneği için, değeri **Varsayılan** veya Devre **Dışı'dan Etkin**olarak değiştirin. **Disabled**</span><span class="sxs-lookup"><span data-stu-id="26b91-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="26b91-108">Tarayıcı penceresinin alt kısmında **Yeniden Başlat'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="26b91-108">At the bottom of the browser window, select **Restart**.</span></span> <br>
 <span data-ttu-id="26b91-109">Değişiklik, Microsoft Edge'i yeniden başlattınktan sonra etkili olur.</span><span class="sxs-lookup"><span data-stu-id="26b91-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="26b91-110">Bu ve dışa aktarma aracını yükleme adımları hakkında bilgi için bkz: [İçerik Arama sonuçlarını dışa aktarma](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="26b91-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>