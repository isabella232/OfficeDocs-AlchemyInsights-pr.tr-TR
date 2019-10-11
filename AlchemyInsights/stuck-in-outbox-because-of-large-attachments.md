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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441325"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="3b6c7-102">Giden Kutusu'nda sıkışmış iletileri düzeltme</span><span class="sxs-lookup"><span data-stu-id="3b6c7-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="3b6c7-103">[Microsoft Destek ve Kurtarma Yardımcısı](https://diagnostics.office.com/#/) aracından ["E-posta iletileri göndermekte, almakta veya bulmakta sorun yaşıyorum"](https://aka.ms/SaRA-OutlookSendReceive) senaryosunu çalıştırarak başlamanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="3b6c7-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="3b6c7-104">Bir ileti Giden Kutunuzda sıkışıp kaldığında, en olası nedenler şunlardır:</span><span class="sxs-lookup"><span data-stu-id="3b6c7-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="3b6c7-105">Büyük ekler.</span><span class="sxs-lookup"><span data-stu-id="3b6c7-105">Large attachments.</span></span>
- <span data-ttu-id="3b6c7-106">Bağlı seçenek **etkinleştirilmediğinde hemen Gönder.**</span><span class="sxs-lookup"><span data-stu-id="3b6c7-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="3b6c7-107">Büyük ekleri kaldırmak için:</span><span class="sxs-lookup"><span data-stu-id="3b6c7-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="3b6c7-108">Outlook'ta,**İşi Çevrimdışı** **Gönder / Al'ı** > seçin.</span><span class="sxs-lookup"><span data-stu-id="3b6c7-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="3b6c7-109">Gezinti bölmesinde Giden **Kutusu'nu**seçin.</span><span class="sxs-lookup"><span data-stu-id="3b6c7-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="3b6c7-110">Buradan şunları yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="3b6c7-110">From here, you can:</span></span> 
    - <span data-ttu-id="3b6c7-111">İletiyi silin (seçin ve sonra **Sil'i**seçin).</span><span class="sxs-lookup"><span data-stu-id="3b6c7-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="3b6c7-112">İletiyi Taslaklar klasörünüze sürükleyin, açmak için çift tıklatın ve eki kaldırın seçin ve sonra **Sil'i**seçin).</span><span class="sxs-lookup"><span data-stu-id="3b6c7-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="3b6c7-113">Outlook'un iletiyi iletmeye çalıştığını belirten bir hata alırsanız, Outlook'u kapatın.</span><span class="sxs-lookup"><span data-stu-id="3b6c7-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="3b6c7-114">Çıkmak birkaç dakika sürebilir.</span><span class="sxs-lookup"><span data-stu-id="3b6c7-114">It may take a few moments to exit.</span></span> <span data-ttu-id="3b6c7-115">Outlook kapanmazsa Ctrl+Alt+Sil tuşuna basın ve **Görev Yöneticisini Başlat'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="3b6c7-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="3b6c7-116">Görev Yöneticisi'nde, **İşlemler** sekmesini seçin, outlook.exe'ye gidin ve **Son İşlem'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="3b6c7-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="3b6c7-117">Outlook kapandıktan sonra yeniden başlatın ve 2 ve 3 adımlarını yineleyin.</span><span class="sxs-lookup"><span data-stu-id="3b6c7-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="3b6c7-118">Eki kaldırdıktan sonra, çevrimiçi çalışmaya devam etmek için**İşI Çevrimdışı** **Gönder /Al'ı** > tıklatın.</span><span class="sxs-lookup"><span data-stu-id="3b6c7-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="3b6c7-119">İletiler, **Gönder'i**tıklattığınızda giden kutuya da takılıp kalır, ancak bağlı değildir.</span><span class="sxs-lookup"><span data-stu-id="3b6c7-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="3b6c7-120">**Gönder / Al'ı** tıklatın ve **Çevrimdışı İş** düğmesine bakın.</span><span class="sxs-lookup"><span data-stu-id="3b6c7-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="3b6c7-121">Eğer maviyse, bağlantın kesilir.</span><span class="sxs-lookup"><span data-stu-id="3b6c7-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="3b6c7-122">Bağlanmak için seçin (düğme beyaza döner) ve **Tümünü Gönder'e**tıklayın.</span><span class="sxs-lookup"><span data-stu-id="3b6c7-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="3b6c7-123">**Bağlandığında hemen Gönder'i**etkinleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="3b6c7-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="3b6c7-124">**Dosya** > **Seçenekleri** >  **Gelişmiş'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="3b6c7-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="3b6c7-125">Gönder **ve al** bölümünde, **bağlandığında hemen Gönder'i**ve ardından **Tamam'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="3b6c7-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="3b6c7-126">Tüm ayrıntılar için bkz:</span><span class="sxs-lookup"><span data-stu-id="3b6c7-126">For full details see:</span></span>
- [<span data-ttu-id="3b6c7-127">Video: Sıkışmış bir e-postayı gönderme veya silme</span><span class="sxs-lookup"><span data-stu-id="3b6c7-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="3b6c7-128">Outlook'ta el ile bir gönderme/alma işlemi başlatana kadar e-posta Giden Kutusu klasöründe kalır</span><span class="sxs-lookup"><span data-stu-id="3b6c7-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
