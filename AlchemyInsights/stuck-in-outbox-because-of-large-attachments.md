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
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241272"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="e55b3-102">Giden Kutusu'nda sıkışmış iletileri düzeltme</span><span class="sxs-lookup"><span data-stu-id="e55b3-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="e55b3-103">[Microsoft Destek ve Kurtarma Yardımcısı](https://diagnostics.office.com/#/) aracından ["E-posta iletileri göndermekte, almakta veya bulmakta sorun yaşıyorum"](https://aka.ms/SaRA-OutlookSendReceive) senaryosunu çalıştırarak başlamanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="e55b3-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="e55b3-104">Giden Kutunuzda bir ileti sıkışıp kaldığında, bunun en olası nedeni büyük bir ek veya "Bağlandığında hemen gönder" seçeneği etkin değildir.</span><span class="sxs-lookup"><span data-stu-id="e55b3-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="e55b3-105">**Büyük eki kaldırma**</span><span class="sxs-lookup"><span data-stu-id="e55b3-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="e55b3-106">Outlook'ta,**İşi Çevrimdışı** **Gönder / Al'ı** > seçin.</span><span class="sxs-lookup"><span data-stu-id="e55b3-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="e55b3-107">Gezinti bölmesinde Giden **Kutusu'nu**seçin.</span><span class="sxs-lookup"><span data-stu-id="e55b3-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="e55b3-108">Buradan şunları yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="e55b3-108">From here, you can:</span></span> 
    - <span data-ttu-id="e55b3-109">İletiyi silin (seçin ve sonra **Sil'i**seçin).</span><span class="sxs-lookup"><span data-stu-id="e55b3-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="e55b3-110">İletiyi Taslaklar klasörünüze sürükleyin, açmak için çift tıklatın ve eki kaldırın seçin ve sonra **Sil'i**seçin).</span><span class="sxs-lookup"><span data-stu-id="e55b3-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="e55b3-111">Outlook'un iletiyi iletmeye çalıştığını belirten bir hata alırsanız, Outlook'u kapatın.</span><span class="sxs-lookup"><span data-stu-id="e55b3-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="e55b3-112">Çıkmak birkaç dakika sürebilir.</span><span class="sxs-lookup"><span data-stu-id="e55b3-112">It may take a few moments to exit.</span></span> <span data-ttu-id="e55b3-113">Outlook kapanmazsa Ctrl+Alt+Sil tuşuna basın ve **Görev Yöneticisini Başlat'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="e55b3-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="e55b3-114">Görev Yöneticisi'nde, **İşlemler** sekmesini seçin, outlook.exe'ye gidin ve **Son İşlem'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="e55b3-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="e55b3-115">Outlook kapandıktan sonra yeniden başlatın ve 2 ve 3 adımlarını yineleyin.</span><span class="sxs-lookup"><span data-stu-id="e55b3-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="e55b3-116">Eki kaldırdıktan sonra, çevrimiçi çalışmaya devam etmek için**İşI Çevrimdışı** **Gönder /Al'ı** > tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e55b3-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="e55b3-117">İletiler, **Gönder'i**tıklattığınızda giden kutuya da takılıp kalır, ancak bağlı değildir.</span><span class="sxs-lookup"><span data-stu-id="e55b3-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="e55b3-118">**Gönder / Al'ı** tıklatın ve **Çevrimdışı İş** düğmesine bakın.</span><span class="sxs-lookup"><span data-stu-id="e55b3-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="e55b3-119">Eğer maviyse, bağlantın kesilir.</span><span class="sxs-lookup"><span data-stu-id="e55b3-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="e55b3-120">Bağlanmak için tıklatın (düğme beyaza döner) ve **Tümünü Gönder'e**tıklayın.</span><span class="sxs-lookup"><span data-stu-id="e55b3-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="e55b3-121">**Bağlıyken hemen Gönder'i etkinleştirin**</span><span class="sxs-lookup"><span data-stu-id="e55b3-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="e55b3-122">Dosya sekmesinde **Seçenekler'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e55b3-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="e55b3-123">Outlook Seçenekleri iletişim kutusunda **Gelişmiş'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e55b3-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="e55b3-124">Gönder ve al bölümünde, **bağlandığında hemen Gönder'i**etkinleştirmek için tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e55b3-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="e55b3-125">**Tamam**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="e55b3-125">Click **OK**.</span></span>
 
<span data-ttu-id="e55b3-126">Tüm ayrıntılar için bkz:</span><span class="sxs-lookup"><span data-stu-id="e55b3-126">For full details, see:</span></span>
- [<span data-ttu-id="e55b3-127">Video: Sıkışmış bir e-postayı gönderme veya silme</span><span class="sxs-lookup"><span data-stu-id="e55b3-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="e55b3-128">Outlook'ta el ile bir gönderme/alma işlemi başlatana kadar e-posta Giden Kutusu klasöründe kalır</span><span class="sxs-lookup"><span data-stu-id="e55b3-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
