---
title: Windows 10'da Windows Bellek Tanılama'yı çalıştırma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358291"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="8d047-102">Windows 10'da Windows Bellek Tanılama'yı çalıştırma</span><span class="sxs-lookup"><span data-stu-id="8d047-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="8d047-103">Bilgisayarınızdaki Windows ve uygulamalar çöküyorsa, donuyorsa veya kararsız bir şekilde hareket ediyorsa, bilgisayarın belleğinde (RAM) sorun yaşayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8d047-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="8d047-104">Bilgisayarın RAM'iyle ilgili sorunları denetlemek için Windows Memory Diagnostic'i çalıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8d047-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="8d047-105">Görev çubuğunuzdaki arama kutusunda **bellek tanılama**yazın ve ardından **Windows Memory Diagnostic'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="8d047-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="8d047-106">Tanılamayı çalıştırmak için bilgisayarın yeniden başlatılması gerekir.</span><span class="sxs-lookup"><span data-stu-id="8d047-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="8d047-107">Hemen yeniden başlatma seçeneğiniz vardır (lütfen önce çalışmanızı kaydedin ve açık belgeleri ve e-postaları kapatın) veya bilgisayarı bir sonraki kez yeniden başlatında otomatik olarak çalışacak tanılamayı zamanlayın:</span><span class="sxs-lookup"><span data-stu-id="8d047-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows Bellek Tanılama](media/windows-memory-diagnostic.png)

<span data-ttu-id="8d047-109">BILGISAYAR yeniden başlatıldığında, **Windows Bellek Tanılama Aracı** otomatik olarak çalışır.</span><span class="sxs-lookup"><span data-stu-id="8d047-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="8d047-110">Durum ve ilerleme tanılama çalıştırılınrken görüntülenir ve klavyenizdeki **ESC** tuşuna basarak tanılamayı iptal etme seçeneğiniz vardır.</span><span class="sxs-lookup"><span data-stu-id="8d047-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="8d047-111">Tanılama tamamlandığında, Windows normal olarak başlar.</span><span class="sxs-lookup"><span data-stu-id="8d047-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="8d047-112">Yeniden başlatmadan hemen sonra, Masaüstü göründüğünde, bellek hataları nın bulunup bulunmadığını belirtmek için bir bildirim (görev çubuğundaki **İşlem Merkezi** simgesinin yanında) görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="8d047-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="8d047-113">Örneğin:</span><span class="sxs-lookup"><span data-stu-id="8d047-113">For example:</span></span>

<span data-ttu-id="8d047-114">İşte İşlem Merkezi simgesi:</span><span class="sxs-lookup"><span data-stu-id="8d047-114">Here's the Action Center icon:</span></span> ![İşlem merkezi simgesi](media/action-center-icon.png) 

<span data-ttu-id="8d047-116">Ve örnek bir bildirim:</span><span class="sxs-lookup"><span data-stu-id="8d047-116">And a sample notification:</span></span> ![Bellek hatası yok](media/no-memory-errors.png)

<span data-ttu-id="8d047-118">Bildirimi kaçırdıysanız, **İşlem Merkezi'ni** görüntülemek ve kaydırılabilir bir bildirim listesini görmek için görev çubuğundaki **İşlem Merkezi** simgesini seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8d047-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="8d047-119">Ayrıntılı bilgileri gözden geçirmek için görev çubuğunuzdaki arama kutusuna **olay** yazın ve ardından **Olay Görüntüleyicisi'ni**seçin.</span><span class="sxs-lookup"><span data-stu-id="8d047-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="8d047-120">Olay **Görüntüleyicisi'nin**sol bölmesinde, **Windows Günlükleri > Sistemi'ne**gidin.</span><span class="sxs-lookup"><span data-stu-id="8d047-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="8d047-121">Sağ bölmede, Kaynak değeri **MemoryDiagnostics-Results**olan olayları görene kadar **Kaynak** sütuna bakarken listeyi aşağı tarayın.</span><span class="sxs-lookup"><span data-stu-id="8d047-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="8d047-122">Bu tür her bir olayı vurgulayın ve listenin altındaki **Genel** sekmesinin altındaki kutuda sonuç bilgilerini görün.</span><span class="sxs-lookup"><span data-stu-id="8d047-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
