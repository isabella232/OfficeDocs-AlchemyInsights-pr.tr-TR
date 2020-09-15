---
title: Explorer ile aç çalışmıyor
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694476"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="cca24-102">Explorer ile aç çalışmıyor</span><span class="sxs-lookup"><span data-stu-id="cca24-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="cca24-103">**Dosya Gezgini 'Nde** gezgin veya Görünüm **ile açıksa** , aşağıdaki adımları izleyerek WebClient hizmetinin **çalışıyor** olarak ayarlandığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="cca24-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="cca24-104">Örneğin, hizmet çalıştırılmamışsa SharePoint veya OneDrive kitaplığının açılması uzun sürebilir.</span><span class="sxs-lookup"><span data-stu-id="cca24-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="cca24-105">Windows Arama kutusuna Çalıştır yazın, masaüstü uygulamasını Çalıştır 'ı seçin, Services. msc yazın ve **ENTER**'u seçin.</span><span class="sxs-lookup"><span data-stu-id="cca24-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="cca24-106">WebClient hizmetine gidip **durum** sütununu denetleyin.</span><span class="sxs-lookup"><span data-stu-id="cca24-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="cca24-107">WebClient hizmeti durumu **çalışmıyorsa**, hizmeti çift tıklatın, **Başlat**'ı ve ardından **Tamam**'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="cca24-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="cca24-108">Gerekirse, **başlatma türü** kutusunda **el ile** veya **Otomatik** 'i seçerek hizmeti etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="cca24-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="cca24-109">Dosya Gezgini 'nde açma sorunlarını gidermek için [, bkz.](https://go.microsoft.com/fwlink/?linkid=871665)</span><span class="sxs-lookup"><span data-stu-id="cca24-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="cca24-110">Daha iyi bir alternatif olarak eşitlemeyi keşfedin: [SharePoint dosyalarını yeni OneDrive eşitleme Istemcisiyle eşitleyin](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="cca24-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

