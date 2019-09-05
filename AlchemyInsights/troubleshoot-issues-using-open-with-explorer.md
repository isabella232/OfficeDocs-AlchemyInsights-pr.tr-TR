---
title: Explorer ile Aç'ı kullanarak sorun giderme sorunları
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
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742753"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="93583-102">Explorer ile Aç ile ilgili sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="93583-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="93583-103">**Explorer ile Aç** komutunu kullanarak SharePoint veya OneDrive'da belge kitaplığı açmayla ilgili sık karşılaşılan sorunları giderin:</span><span class="sxs-lookup"><span data-stu-id="93583-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="93583-104">Internet Explorer 10 veya Internet Explorer 11'i kullanın.</span><span class="sxs-lookup"><span data-stu-id="93583-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="93583-105">**Explorer ile açık** Microsoft Edge, Google Chrome, Firefox ve diğerleri ile uyumlu değildir.</span><span class="sxs-lookup"><span data-stu-id="93583-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="93583-106">**Explorer ile açık** Internet Explorer dışındaki tüm tarayıcılarda devre dışı bırakılır.</span><span class="sxs-lookup"><span data-stu-id="93583-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="93583-107">**Explorer ile açık** SharePoint kitaplıkları için modern deneyim kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="93583-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="93583-108">Bunun yerine **Dosya Gezgini'nde** Görünüm'i kullanın.</span><span class="sxs-lookup"><span data-stu-id="93583-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="93583-109">**Dosya Gezgini'nde Görünüm** **seçeneklerini** \> seçin.</span><span class="sxs-lookup"><span data-stu-id="93583-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="93583-110">Dosya Gezgini'nde Görünüm Microsoft Edge, Google Chrome, Firefox ve diğer leriyle uyumlu değildir.</span><span class="sxs-lookup"><span data-stu-id="93583-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="93583-111">Yalnızca Internet Explorer'da kullanılabilir dosya **gezgininde görüntüle.**</span><span class="sxs-lookup"><span data-stu-id="93583-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="93583-112">WebClient hizmetinin çalışırken olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="93583-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="93583-113">Windows arama kutusunda çalıştır yazın, Çalıştır masaüstü uygulamasını seçin, services.msc yazın ve ardından Enter tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="93583-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="93583-114">WebClient hizmetine gidin ve **Durum** sütununda "Çalışan" görüntülediğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="93583-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="93583-115">Değilse, hizmeti çift tıklatın, Başlat'ı \*\*\*\* tıklatın ve sonra **Tamam'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="93583-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="93583-116">(Önce **Başlangıç türü** kutusunda **Manuel** veya Otomatik'i seçerek hizmeti etkinleştirmeniz gerekebilir.) \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="93583-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="93583-117">Dosya Gezgini'nde kitaplık açmak, birden çok dosya ve klasörü bir kez kopyalamanız veya taşımanız gerekiyorsa kullanışlıdır, ancak kitaplıkta düzenli olarak çalışmak istiyorsanız, eşitleme nizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="93583-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="93583-118">Dosya Gezgini'nde açılan sorunları gidermek için [Explorer'da](https://go.microsoft.com/fwlink/?linkid=871665)Aç'a bakın.</span><span class="sxs-lookup"><span data-stu-id="93583-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="93583-119">Eşitleme ayarlama hakkında daha fazla bilgi için, [yeni OneDrive eşitleme istemcisi ile Eşitleme SharePoint](https://go.microsoft.com/fwlink/?linkid=871666)dosyalarına bakın.</span><span class="sxs-lookup"><span data-stu-id="93583-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="93583-120">Daha fazla bilgi için [SharePoint Online'daki sorunları gidermek için lütfen "Explorer ile Aç" komutunu nasıl kullanacağınızı](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) makaleye bakın.</span><span class="sxs-lookup"><span data-stu-id="93583-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

