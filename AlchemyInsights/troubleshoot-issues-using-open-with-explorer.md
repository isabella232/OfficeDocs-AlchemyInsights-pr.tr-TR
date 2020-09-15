---
title: Explorer ile aç 'ı kullanarak sorunları giderme
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659078"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="c1e4a-102">Explorer ile aç sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="c1e4a-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="c1e4a-103">SharePoint veya OneDrive 'da belge kitaplığı açma ile ilgili sık karşılaşılan sorunları, **Explorer Ile aç** komutunu kullanarak Düzeltme:</span><span class="sxs-lookup"><span data-stu-id="c1e4a-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="c1e4a-104">Internet Explorer 10 veya Internet Explorer 11 kullanın.</span><span class="sxs-lookup"><span data-stu-id="c1e4a-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="c1e4a-105">**Explorer Ile aç** , Microsoft Edge, Google Chrome, Firefox ve diğer kişilerle uyumlu değildir.</span><span class="sxs-lookup"><span data-stu-id="c1e4a-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="c1e4a-106">Internet Explorer dışında tüm tarayıcılarda **Explorer Ile aç** özelliği devre dışı bırakılmıştır.</span><span class="sxs-lookup"><span data-stu-id="c1e4a-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="c1e4a-107">SharePoint kitaplıkları için modern deneyimde **Explorer Ile aç** özelliği kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="c1e4a-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="c1e4a-108">Bunun yerine **Dosya Gezgini 'Nde görünüm** kullanın.</span><span class="sxs-lookup"><span data-stu-id="c1e4a-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="c1e4a-109">**View options** \> **Dosya Gezgini 'nde**görünüm seçenekleri görünümünü seçin.</span><span class="sxs-lookup"><span data-stu-id="c1e4a-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="c1e4a-110">Dosya Gezgini 'ndeki görünüm, Microsoft Edge, Google Chrome, Firefox ve diğer kişilerle uyumlu değildir.</span><span class="sxs-lookup"><span data-stu-id="c1e4a-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="c1e4a-111">**Dosya Gezgini** 'Nde yalnızca Internet Explorer 'da kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="c1e4a-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="c1e4a-112">WebClient hizmetinin çalıştığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="c1e4a-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="c1e4a-113">Windows Arama kutusuna Çalıştır yazın, masaüstü uygulamasını Çalıştır 'ı seçin, Services. msc yazın ve ENTER tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="c1e4a-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="c1e4a-114">WebClient hizmetine gidin ve **durum** sütununda "çalışıyor" olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="c1e4a-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="c1e4a-115">Desteklemiyorsa, hizmeti çift tıklatın, **Başlat**'ı ve ardından **Tamam**'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="c1e4a-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="c1e4a-116">( **Başlangıç türü** kutusunda **el ile** veya **Otomatik** 'i seçerek hizmeti etkinleştirmeniz gerekebilir.)</span><span class="sxs-lookup"><span data-stu-id="c1e4a-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="c1e4a-117">Bir kitaplığı dosya Gezgini 'nde açmak, birden çok dosya ve klasörü bir kez kopyalamanız veya taşımanız gerekiyorsa kullanışlıdır, ancak kitaplıkta düzenli olarak çalışmak istiyorsanız, eşitlemeyi öneririz.</span><span class="sxs-lookup"><span data-stu-id="c1e4a-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="c1e4a-118">Dosya Gezgini 'nde açma sorunlarını gidermek için [, bkz.](https://go.microsoft.com/fwlink/?linkid=871665)</span><span class="sxs-lookup"><span data-stu-id="c1e4a-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="c1e4a-119">Eşitlemeyi ayarlama hakkında bilgi için, [SharePoint dosyalarını yeni OneDrive eşitleme Istemcisiyle eşitleme](https://go.microsoft.com/fwlink/?linkid=871666)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="c1e4a-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="c1e4a-120">Daha fazla bilgi için [SharePoint Online 'daki sorunları gidermek üzere "Gezgin Ile aç" komutunun nasıl kullanılacağı](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) makalesine bakın.</span><span class="sxs-lookup"><span data-stu-id="c1e4a-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

