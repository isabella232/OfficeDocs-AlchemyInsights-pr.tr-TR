---
title: Explorer ile Aç'ı çalışmıyor
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29494165"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="001fd-102">Explorer ile Aç'ı çalışmıyor</span><span class="sxs-lookup"><span data-stu-id="001fd-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="001fd-p101">**Explorer ile Aç** ' ı veya **Dosya Gezgini görünümünde** işe yaramazsa WebClient hizmetini **çalıştıran** aşağıdaki adımları izleyerek ayarlandığından emin olun. Örneğin, bu hizmeti çalışmadığı zamanlarda bir OneDrive ya da SharePoint kitaplığı açmak için uzun zaman alabilir.</span><span class="sxs-lookup"><span data-stu-id="001fd-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="001fd-105">Windows Arama kutusuna türü çalıştırmak, çalışma Masaüstü uygulama, services.msc yazın ve sonra **Enter**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="001fd-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="001fd-p102">WebClient hizmetini aşağı doğru kaydırma yapın ve **Durum** sütununu denetleyin. WebClient hizmeti durum **çalışan**değilse, hizmeti çift tıklatın, **Başlat**' ı tıklatın ve sonra **Tamam**' ı tıklatın. Gerekirse, **el ile** veya **Otomatik** **Başlangıç türü** kutusunda seçerek hizmeti etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="001fd-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="001fd-p103">Dosya Gezgini'nde açma sorunlarını gidermek için [Explorer'da açık](https://go.microsoft.com/fwlink/?linkid=871665)bakın. Daha iyi bir alternatif olarak eşitleme keşfedin: [Yeni OneDrive eşitleme istemcisi ile eşitleme SharePoint dosyaları](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="001fd-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

