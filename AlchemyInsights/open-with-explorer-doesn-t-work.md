---
title: Explorer ile açık çalışmıyor
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713054"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="09874-102">Explorer ile Açık çalışmıyor</span><span class="sxs-lookup"><span data-stu-id="09874-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="09874-103">**Explorer'da Aç** veya **Dosya Gezgini'nde Görünüm** çalışmıyorsa, WebClient hizmetinin aşağıdaki adımları izleyerek **Çalıştırma** olarak ayarlandığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="09874-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="09874-104">Örneğin, hizmet çalışmadığında SharePoint veya OneDrive kitaplığını açmak uzun sürebilir.</span><span class="sxs-lookup"><span data-stu-id="09874-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="09874-105">Windows arama kutusunda çalıştır yazın, Çalıştır masaüstü uygulamasını seçin, services.msc yazın ve sonra **Enter'u**seçin.</span><span class="sxs-lookup"><span data-stu-id="09874-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="09874-106">WebClient hizmetine gidin ve **Durum** sütununa bakın.</span><span class="sxs-lookup"><span data-stu-id="09874-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="09874-107">WebClient hizmet durumu **Çalışmıyorsa,** hizmeti çift tıklatın, **Başlat'ı**tıklatın ve ardından **Tamam'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="09874-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="09874-108">**Başlangıç türü** kutusunda **Manuel** veya **Otomatik'i** seçerek gerekirse hizmeti etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="09874-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="09874-109">Dosya Gezgini'nde açılan sorunları gidermek için [Explorer'da Aç'a](https://go.microsoft.com/fwlink/?linkid=871665)bakın.</span><span class="sxs-lookup"><span data-stu-id="09874-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="09874-110">Daha iyi bir alternatif olarak eşitlemeyi keşfedin: [SharePoint dosyalarını yeni OneDrive eşitleme istemcisiyle eşitleyin.](https://go.microsoft.com/fwlink/?linkid=871666)</span><span class="sxs-lookup"><span data-stu-id="09874-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

