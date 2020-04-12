---
title: Büyük ekler nedeniyle Giden Kutusu'nda sıkışmış
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232650"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="e3ef0-102">Giden Kutusu'nda sıkışmış iletileri düzeltme</span><span class="sxs-lookup"><span data-stu-id="e3ef0-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="e3ef0-103">Etkilenen makinedeki [Microsoft Destek ve Kurtarma Yardımcısı](https://diagnostics.office.com/#/) aracından ["E-posta iletileri göndermekte, almakta veya bulmakta sorun yaşıyorum"](https://aka.ms/SaRA-OutlookSendReceive) senaryosunu çalıştırarak başlamanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="e3ef0-104">Giden Kutunuzda bir ileti sıkışıp kaldığında, bunun en olası nedeni büyük bir ek veya "Bağlandığında hemen gönder" seçeneği etkin değildir.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="e3ef0-105">**Büyük eki kaldırma**</span><span class="sxs-lookup"><span data-stu-id="e3ef0-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="e3ef0-106">**İşi Çevrimdışı** **Gönder / Al'ı** > tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="e3ef0-107">Gezinti **bölmesinde, Giden Kutusu'nu**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="e3ef0-108">Buradan şunları yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="e3ef0-108">From here, you can:</span></span> 
    - <span data-ttu-id="e3ef0-109">İletiyi silin.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-109">Delete the message.</span></span> <span data-ttu-id="e3ef0-110">Sadece seçin ve **Sil'e**tıklayın.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="e3ef0-111">İletiyi **taslaklar klasörünüze**sürükleyin, iletiyi açmak için çift tıklatın ve eki silin (tıklatın ve **Sil'i**tıklatın).</span><span class="sxs-lookup"><span data-stu-id="e3ef0-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="e3ef0-112">Bir hata size Outlook'un iletiyi iletmeye çalıştığını söylüyorsa, Outlook'u kapatın.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="e3ef0-113">Çıkmak birkaç dakika sürebilir.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-113">It may take a few moments to exit.</span></span> <span data-ttu-id="e3ef0-114">Outlook kapanmazsa **Ctrl+Alt+Sil** tuşuna basın ve **Görev Yöneticisini Başlat'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="e3ef0-115">Görev Yöneticisi'nde, **İşlemler** sekmesini seçin, outlook.exe'ye gidin ve **Son İşlem'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="e3ef0-116">Outlook kapandıktan sonra Outlook'u yeniden başlatın ve 2-3 adımlarını yineleyin.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="e3ef0-117">Eki kaldırdıktan sonra, düğmeyi seçmek ve çevrimiçi çalışmaya devam etmek için **Çevrimdışı Gönder /Al'ı** > **Work Offline** tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="e3ef0-118">İletiler, **Gönder'i**tıklattığınızda giden kutuya da takılıp kalır, ancak bağlı değildir.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="e3ef0-119">**Gönder / Al'ı** tıklatın ve **Çevrimdışı İş** düğmesine bakın.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="e3ef0-120">Eğer maviyse, bağlantın kesilir.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="e3ef0-121">Bağlanmak için tıklatın (düğme beyaza döner) ve **Tümünü Gönder'e**tıklayın.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="e3ef0-122">**Bağlıyken hemen Gönder'i etkinleştirin**</span><span class="sxs-lookup"><span data-stu-id="e3ef0-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="e3ef0-123">Dosya sekmesinde **Seçenekler'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="e3ef0-124">Outlook Seçenekleri iletişim kutusunda **Gelişmiş'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="e3ef0-125">Gönder ve al bölümünde, **bağlandığında hemen Gönder'i**etkinleştirmek için tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="e3ef0-126">**Tamam**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="e3ef0-126">Click **OK**.</span></span>
 
<span data-ttu-id="e3ef0-127">Tüm ayrıntılar için bkz:</span><span class="sxs-lookup"><span data-stu-id="e3ef0-127">For full details, see:</span></span>
- [<span data-ttu-id="e3ef0-128">Video: Sıkışmış bir e-postayı gönderme veya silme</span><span class="sxs-lookup"><span data-stu-id="e3ef0-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="e3ef0-129">Outlook'ta el ile bir gönderme/alma işlemi başlatana kadar e-posta Giden Kutusu klasöründe kalır</span><span class="sxs-lookup"><span data-stu-id="e3ef0-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
