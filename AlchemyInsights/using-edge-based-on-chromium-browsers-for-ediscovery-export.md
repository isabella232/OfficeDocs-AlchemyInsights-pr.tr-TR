---
title: EBulma dışarı aktarma için Kmıum tarayıcılarında Microsoft Edge kullanma
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
- "3473"
- "3100022"
ms.openlocfilehash: 64aebb7f048dba37eef8cd1fa6286b36823d3f0f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734535"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="8b7ac-102">EBulma dışarı aktarma için Kmıum tarayıcılarında Microsoft Edge kullanma</span><span class="sxs-lookup"><span data-stu-id="8b7ac-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="8b7ac-103">Son değişiklik nedeniyle, Microsoft Edge tarayıcılarında artık ClickOnce desteği varsayılan olarak etkin olmayacaktır.</span><span class="sxs-lookup"><span data-stu-id="8b7ac-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="8b7ac-104">Microsoft 365 eBulma dışarı aktarma aracı 'nı kullanmaya devam etmek için Microsoft Internet Explorer kullanmanız veya Microsoft Edge 'de ClickOnce desteğini etkinleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="8b7ac-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="8b7ac-105">Microsoft Edge 'de, Kmıum 'a dayalı ClickOnce desteğini etkinleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="8b7ac-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="8b7ac-106">Microsoft Edge tarayıcınızda, edge://flags/#edge-Tıklat-bir kez ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="8b7ac-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="8b7ac-107">ClickOnce desteği seçeneği için, değeri **varsayılan** veya **devre dışı bırakılmış** olarak **değiştirin.**</span><span class="sxs-lookup"><span data-stu-id="8b7ac-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="8b7ac-108">Tarayıcı penceresinin en altında **Yeniden Başlat**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="8b7ac-108">At the bottom of the browser window, select **Restart**.</span></span> <br>
 <span data-ttu-id="8b7ac-109">Değişiklik, Microsoft Edge yeniden başlatıldıktan sonra etkinleşir.</span><span class="sxs-lookup"><span data-stu-id="8b7ac-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="8b7ac-110">Bu bilgiler ve dışarı aktarma aracı yükleme adımları için bkz: [ Içerik arama sonuçlarını dışarı aktarma](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="8b7ac-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>