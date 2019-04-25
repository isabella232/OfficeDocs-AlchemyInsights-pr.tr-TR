---
title: Explorer ile Aç'ı kullanarak sorunları giderme
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390627"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="8cdc8-102">Açık Explorer ile ilgili sorunları çözün</span><span class="sxs-lookup"><span data-stu-id="8cdc8-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="8cdc8-103">OneDrive **Explorer ile Aç** komutunu kullanarak veya SharePoint belge kitaplığı açarak sık karşılaşılan sorunları giderir:</span><span class="sxs-lookup"><span data-stu-id="8cdc8-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="8cdc8-104">Internet Explorer 10 veya 11 Internet Explorer'ı kullanın.</span><span class="sxs-lookup"><span data-stu-id="8cdc8-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="8cdc8-105">**Explorer ile Aç** Microsoft Edge, Google Chrome, Firefox ve diğerleri ile uyumlu değildir.</span><span class="sxs-lookup"><span data-stu-id="8cdc8-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="8cdc8-106">**Explorer ile Aç** Internet Explorer dışındaki tüm tarayıcılarda devre dışı bırakılır.</span><span class="sxs-lookup"><span data-stu-id="8cdc8-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="8cdc8-107">**Explorer ile Aç** modern deneyimi SharePoint kitaplıkları için kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="8cdc8-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="8cdc8-108">Bunun yerine **Dosya Explorer görünümü'nü** kullanın.</span><span class="sxs-lookup"><span data-stu-id="8cdc8-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="8cdc8-109">**Görünüm seçeneklerini** seçin \> **Dosya Gezgini görünümünde**.</span><span class="sxs-lookup"><span data-stu-id="8cdc8-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="8cdc8-110">Dosya Gezgini görünümünde Microsoft Edge, Google Chrome, Firefox ve diğerleri ile uyumlu değil.</span><span class="sxs-lookup"><span data-stu-id="8cdc8-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="8cdc8-111">**Dosya Gezgini görünümünde** yalnızca Internet Explorer'da kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="8cdc8-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="8cdc8-112">WebClient hizmetinin çalıştığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="8cdc8-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="8cdc8-113">Windows Arama kutusunda, çalıştırmak, tür çalışma Masaüstü app seçin, services.msc yazın ve Enter tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="8cdc8-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="8cdc8-114">WebClient hizmetini aşağı doğru kaydırın ve **Durum** sütununda "Çalışan" görüntülediğinden emin olun</span><span class="sxs-lookup"><span data-stu-id="8cdc8-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="8cdc8-115">Seçili değilse, hizmeti çift tıklatın, **Başlat**' ı tıklatın ve sonra **Tamam**' ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="8cdc8-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="8cdc8-116">( **El ile** veya **Otomatik** **Başlangıç türü** kutusunda seçerek önce hizmeti etkinleştirmeniz gerekebilir.)</span><span class="sxs-lookup"><span data-stu-id="8cdc8-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="8cdc8-117">Dosya Gezgini'nde bir kitaplığı açmak, kopyalamak veya bir kez, ancak düzenli olarak kütüphanede çalışmak istiyorsanız, birden çok dosya ve klasörleri taşımak gerekiyorsa kullanışlıdır, onu eşitlemeyi öneririz.</span><span class="sxs-lookup"><span data-stu-id="8cdc8-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="8cdc8-118">Dosya Gezgini'nde açma sorunlarını gidermek için [Explorer'da açık](https://go.microsoft.com/fwlink/?linkid=871665)bakın.</span><span class="sxs-lookup"><span data-stu-id="8cdc8-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="8cdc8-119">[Yeni OneDrive eşitleme istemcisi ile eşitleme SharePoint dosyaları](https://go.microsoft.com/fwlink/?linkid=871666)eşitleme ayarlama hakkında daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="8cdc8-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="8cdc8-120">Lütfen daha fazla bilgi için [SharePoint çevrimiçi sorunlarını giderme "Explorer açık olan" komutunun nasıl kullanılacağını](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) makalesine bakın.</span><span class="sxs-lookup"><span data-stu-id="8cdc8-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

