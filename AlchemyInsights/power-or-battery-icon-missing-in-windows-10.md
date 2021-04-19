---
title: Windows 10'da güç veya pil simgesi eksik
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790568"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="39b06-102">Windows 10'da güç veya pil simgesi eksik</span><span class="sxs-lookup"><span data-stu-id="39b06-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="39b06-103">Windows 10 cihazınızın pili varsa (örneğin, dizüstü bilgisayar veya tablet veya UPS'e USB ile bağlı bir bilgisayar), normalde saatin yakınında görev çubuğunda bir güç/pil simgesi gösterilir; örneğin:</span><span class="sxs-lookup"><span data-stu-id="39b06-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Pil simgesi](media/battery-icon.png)

<span data-ttu-id="39b06-105">Bu simgeyi görmüyorsanız gizlenmiş olabilir:</span><span class="sxs-lookup"><span data-stu-id="39b06-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="39b06-106">Görev çubuğunda **[Ayarlar > Kişiselleştirme > gidin.](ms-settings:taskbar?activationSource=GetHelp)**</span><span class="sxs-lookup"><span data-stu-id="39b06-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="39b06-107">Bildirim alanında Görev çubuğunda görünecek **simgeleri seçin seçeneğine tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="39b06-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="39b06-108">Ardından listede **Güç** öğesini bulun ve bu öğenin ayarını Açık olarak **değiştir.**</span><span class="sxs-lookup"><span data-stu-id="39b06-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Görev çubuğundaki güç simgesini göster](media/power-icon-on.png)

<span data-ttu-id="39b06-110">**Sorun giderme**</span><span class="sxs-lookup"><span data-stu-id="39b06-110">**Troubleshooting**</span></span>

<span data-ttu-id="39b06-111">Yukarıdaki yönergeleri izlediysanız ve **Güç** geçiş düğmesi gri görünüyor veya görünmüyorsa, görev çubuğundaki arama kutusuna  cihaz yöneticisi yazın ve ardından sonuç listesinde Cihaz Yöneticisi'ni seçin.</span><span class="sxs-lookup"><span data-stu-id="39b06-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="39b06-112">Piller **altında** cihazınızın pil seçeneğine sağ tıklayın, Devre dışı bırak'a **ve** Evet'e **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="39b06-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="39b06-113">Birkaç saniye bekleyin, ardından pile sağ tıklayın ve Etkinleştir'e **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="39b06-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="39b06-114">Ardından cihazınızı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="39b06-114">Then restart your device.</span></span>

<span data-ttu-id="39b06-115">Yukarıdaki yönergeleri izlediysiniz ancak pil simgesi görev çubuğunda görünmüyorsa görev çubuğundaki arama kutusuna görev yöneticisi  yazın ve ardından sonuç listesinde Görev Yöneticisi'ne tıklayın.</span><span class="sxs-lookup"><span data-stu-id="39b06-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="39b06-116">İşlemler **sekmesindeki** Ad'ın **altında Gezgin'e** sağ **tıklayın ve** yeniden başlat'a **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="39b06-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
