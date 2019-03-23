---
title: Explorer ile Aç'ı çalışmıyor
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30764928"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="20072-102">Explorer ile Aç'ı çalışmıyor</span><span class="sxs-lookup"><span data-stu-id="20072-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="20072-103">**Explorer ile Aç** ' ı veya **Dosya Gezgini görünümünde** işe yaramazsa WebClient hizmetini **çalıştıran** aşağıdaki adımları izleyerek ayarlandığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="20072-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="20072-104">Örneğin, bu hizmeti çalışmadığı zamanlarda bir OneDrive ya da SharePoint kitaplığı açmak için uzun zaman alabilir.</span><span class="sxs-lookup"><span data-stu-id="20072-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="20072-105">Windows Arama kutusuna türü çalıştırmak, çalışma Masaüstü uygulama, services.msc yazın ve sonra **Enter**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="20072-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="20072-106">WebClient hizmetini aşağı doğru kaydırma yapın ve **Durum** sütununu denetleyin.</span><span class="sxs-lookup"><span data-stu-id="20072-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="20072-107">WebClient hizmeti durum **çalışan**değilse, hizmeti çift tıklatın, **Başlat**' ı tıklatın ve sonra **Tamam**' ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="20072-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="20072-108">Gerekirse, **el ile** veya **Otomatik** **Başlangıç türü** kutusunda seçerek hizmeti etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="20072-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="20072-109">Dosya Gezgini'nde açma sorunlarını gidermek için [Explorer'da açık](https://go.microsoft.com/fwlink/?linkid=871665)bakın.</span><span class="sxs-lookup"><span data-stu-id="20072-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="20072-110">Daha iyi bir alternatif olarak eşitleme keşfedin: [Yeni OneDrive eşitleme istemcisi ile eşitleme SharePoint dosyaları](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="20072-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

