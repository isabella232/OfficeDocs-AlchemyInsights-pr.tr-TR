---
title: Windows 10'da Windows Bellek Tanılama'yı çalıştırma
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
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826687"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="328f1-102">Windows 10'da Windows Bellek Tanılama'yı çalıştırma</span><span class="sxs-lookup"><span data-stu-id="328f1-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="328f1-103">Bilgisayarınızda Windows ve uygulamalar kilitlenmeye, donuyorsa veya kararsız bir şekilde davranıyorsa, bilgisayarınızın belleğinde (RAM) bir sorun olabilir.</span><span class="sxs-lookup"><span data-stu-id="328f1-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="328f1-104">Bilgisayarınızın RAM'iyle ilgili sorunları kontrol etmek için Windows Bellek Tanılama'yı çalıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="328f1-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="328f1-105">Görev çubuğunuzda arama kutusuna bellek tanılama **yazın ve** ardından Windows Bellek **Tanılama'yı seçin.**</span><span class="sxs-lookup"><span data-stu-id="328f1-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="328f1-106">Tanılamayı çalıştırmak için bilgisayarın yeniden başlatılması gerekiyor.</span><span class="sxs-lookup"><span data-stu-id="328f1-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="328f1-107">Hemen yeniden başlatma seçeneğiniz vardır (lütfen çalışmanızı kaydedin ve önce açık belgeleri ve e-postaları kapatın) veya bilgisayarı bir sonraki yeniden başlatma işlemi sırasında tanılamanın otomatik olarak çalışacak şekilde zamanlamayı deneyin:</span><span class="sxs-lookup"><span data-stu-id="328f1-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows Hafıza Tanılama](media/windows-memory-diagnostic.png)

<span data-ttu-id="328f1-109">Bilgisayar yeniden başlatıldığında Windows Bellek **Tanılama Aracı otomatik** olarak çalışır.</span><span class="sxs-lookup"><span data-stu-id="328f1-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="328f1-110">Tanılamalar çalıştırılıyorken durum ve ilerleme durumu görüntülenir ve klavyenizde **ESC** tuşuna basarak tanılamayı iptal seçeneğiniz vardır.</span><span class="sxs-lookup"><span data-stu-id="328f1-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="328f1-111">Tanılama tamamlandığında, Windows normal şekilde başlar.</span><span class="sxs-lookup"><span data-stu-id="328f1-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="328f1-112">Yeniden başlatmanın hemen ardından Masaüstü görüntülendiğinde, herhangi  bir bellek hatası bulunıp buluna olmadığını göstermek için bir bildirim (görev çubuğundaki İşlem Merkezi simgesinin yanında) gösterilir.</span><span class="sxs-lookup"><span data-stu-id="328f1-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="328f1-113">Örneğin:</span><span class="sxs-lookup"><span data-stu-id="328f1-113">For example:</span></span>

<span data-ttu-id="328f1-114">İşte İşlem Merkezi simgesi:</span><span class="sxs-lookup"><span data-stu-id="328f1-114">Here's the Action Center icon:</span></span> ![İşlem merkezi simgesi](media/action-center-icon.png) 

<span data-ttu-id="328f1-116">Ve örnek bir bildirim:</span><span class="sxs-lookup"><span data-stu-id="328f1-116">And a sample notification:</span></span> ![Bellek hatası yok](media/no-memory-errors.png)

<span data-ttu-id="328f1-118">Bildirimi kaçırdıysanız, İşlem Merkezi'yi görüntülemek ve kaydırılabilir  bir bildirim listesi görmek için görev çubuğunda İşlem Merkezi simgesini seçebilirsiniz. </span><span class="sxs-lookup"><span data-stu-id="328f1-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="328f1-119">Ayrıntılı bilgileri gözden geçirmek için, **görev çubuğunuzda** arama kutusuna olayı yazın ve ardından Olay **Görüntüleyicisi'ni seçin.**</span><span class="sxs-lookup"><span data-stu-id="328f1-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="328f1-120">Olay **Görüntüleyicisi'nin** sol bölmesinde, Windows Günlükleri ve **Sistem > gidin.**</span><span class="sxs-lookup"><span data-stu-id="328f1-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="328f1-121">Sağ bölmede, Kaynak sütununa bakarak listeyi  aşağı doğru tarayın; Kaynak değeri **MemoryDiagnostics-Results** ile ilgili olayları görene kadar.</span><span class="sxs-lookup"><span data-stu-id="328f1-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="328f1-122">Bu tür olayları vurgulayın ve listenin altındaki Genel sekmesinin **altındaki** kutuda sonuç bilgilerini görüntüleyin.</span><span class="sxs-lookup"><span data-stu-id="328f1-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
