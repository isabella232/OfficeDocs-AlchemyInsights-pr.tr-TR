---
title: Office dosyasını çift tıklatmak dosyayı açamaz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812099"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="7c15c-102">Office dosyasını çift tıklatmak dosyayı açamaz</span><span class="sxs-lookup"><span data-stu-id="7c15c-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="7c15c-103">Bir Office dosyasını çift tıklattıktan sonra, programın açık olduğunu ancak dosyanın kendisinin açık olmadığını görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7c15c-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="7c15c-104">Veya şu hatayı alabilirsiniz: "komut programa gönderilirken bir sorun oluştu."</span><span class="sxs-lookup"><span data-stu-id="7c15c-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="7c15c-105">Bunun birçok nedeni vardır, ancak en yaygın iki çözüm bulunmaktadır:</span><span class="sxs-lookup"><span data-stu-id="7c15c-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="7c15c-106">Excel içinden, DDE seçeneğinin işaretlenmemiş olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="7c15c-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="7c15c-107">Bu seçenek, yeni bir çalışma kitabı oluşturularak ve **gelişmiş > dosya > seçenekleri**seçilerek bulunabilir.</span><span class="sxs-lookup"><span data-stu-id="7c15c-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="7c15c-108">**Genel** bölümünde, **dinamik VERI değişimi (DDE) kullanan diğer uygulamaları yoksay**seçeneğinin işaretini kaldırın.</span><span class="sxs-lookup"><span data-stu-id="7c15c-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="7c15c-109">Varsayılan ayarları geri yüklemek için çevrimiçi onarım 'ı çalıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7c15c-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="7c15c-110">Windows Başlat düğmesine tıklayın ve "Denetim Masası" nı arayın.</span><span class="sxs-lookup"><span data-stu-id="7c15c-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="7c15c-111">**Denetim Masası**'nı açın ve programlar **> programlar ve Özellikler**'e gidin.</span><span class="sxs-lookup"><span data-stu-id="7c15c-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="7c15c-112">Ardından **Microsoft Office [sürüm]** öğesine sağ tıklayın ve **Çevrimiçi onarım > Değiştir**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="7c15c-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="7c15c-113">Bu çözümlerden hiçbirisi işe yaramazsa, destek makalesinde daha eksiksiz bir çözüm listesi bulunabilir, bir [Office dosyasını çift tıklatarak açamaz](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="7c15c-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
