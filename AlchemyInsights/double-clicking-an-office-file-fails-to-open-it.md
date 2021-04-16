---
title: Bir Office dosyasına çift tık başarısız olan dosya açamıyor
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814825"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="28868-102">Bir Office dosyasına çift tık başarısız olan dosya açamıyor</span><span class="sxs-lookup"><span data-stu-id="28868-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="28868-103">Bir Office dosyasına çift tıklarsanız, programın açık olduğunu ama dosyanın kendisini açmadıyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="28868-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="28868-104">Ya da şu hatayı alabilirsiniz: "Komutu programa gönderirken bir sorun oluştu."</span><span class="sxs-lookup"><span data-stu-id="28868-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="28868-105">Bunun birçok nedeni vardır, ancak en yaygın iki çözüm vardır:</span><span class="sxs-lookup"><span data-stu-id="28868-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="28868-106">Excel'in içinde, DDE seçeneğinin işaretsiz olduğundan emin olur.</span><span class="sxs-lookup"><span data-stu-id="28868-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="28868-107">Bu seçenek, yeni bir çalışma kitabı oluşturarak ve sonra Dosya Seçenekleri > **Ve Gelişmiş > bulunabilir.**</span><span class="sxs-lookup"><span data-stu-id="28868-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="28868-108">Genel **bölümünde,** Dinamik Veri Değişimi **(DDE) kullanan diğer uygulamaları yoksay'ın işaretini kaldırın.**</span><span class="sxs-lookup"><span data-stu-id="28868-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="28868-109">Varsayılan ayarları geri yüklemek için Çevrimiçi Onarım'i çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="28868-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="28868-110">Windows Başlat düğmesine tıklayın ve "Denetim Masası" ifadesini aratır.</span><span class="sxs-lookup"><span data-stu-id="28868-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="28868-111">Denetim **Masası'nı açın** ve Programlar ve **Özellikler > gidin.**</span><span class="sxs-lookup"><span data-stu-id="28868-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="28868-112">Ardından Microsoft **Office [Sürüm] üzerine sağ tıklayın ve Çevrimiçi** **Onarım'da > öğesini seçin.**</span><span class="sxs-lookup"><span data-stu-id="28868-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="28868-113">Bu çözümlerden hiçbiri işe yaramazsa, Office dosyasına çift tıklandıktan sonra dosya açılmaya çalışamaz. Destek makalesinde çözümlerin [daha eksiksiz bir listesi bulunabilir.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="28868-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
