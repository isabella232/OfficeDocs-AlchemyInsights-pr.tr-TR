---
title: Yazdırma Biriktiricisi sorunu çözüldü
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801861"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="bf597-102">Yazdırma Biriktiricisi sorunu çözüldü</span><span class="sxs-lookup"><span data-stu-id="bf597-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="bf597-103">Cihazınız Windows 10  **Işletim sistemi derleme 19041,329**ile güncelleştirildiyse, bazı yazıcıların yazdırmasının başarısız olduğu bir sorunu gözlemlediniz.</span><span class="sxs-lookup"><span data-stu-id="bf597-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="bf597-104">Yazdırma Biriktiricisi bir hata oluşturabilir veya yazdırmaya çalışırken beklenmedik bir şekilde kapatılabilir ve etkilenen yazıcıdan hiçbir çıkış alınmaz.</span><span class="sxs-lookup"><span data-stu-id="bf597-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="bf597-105">Bu sorun, işletim sistemi derleme  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="bf597-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="bf597-106">**Devam eden araştırma**</span><span class="sxs-lookup"><span data-stu-id="bf597-106">**Ongoing investigation**</span></span>

<span data-ttu-id="bf597-107">Yerel güvenlik yetkilisi alt sistemi hizmeti (LSASS) dosyası (**Isass.exe**), "kritik sistem işlemi, C:\WINDOWS\system32\Isass.exe durum koduyla başarısız olan" kritik sistem işlemi başarısız olabilir.</span><span class="sxs-lookup"><span data-stu-id="bf597-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="bf597-108">Makine şimdi yeniden başlatılmalıdır ".</span><span class="sxs-lookup"><span data-stu-id="bf597-108">The machine must now be restarted".</span></span>  <span data-ttu-id="bf597-109">**Microsoft bir çözüm üzerinde çalışmaktadır ve yakında piyasaya çıkacak bir sürümde güncelleştirme sağlayacaktır.**</span><span class="sxs-lookup"><span data-stu-id="bf597-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="bf597-110">Daha fazla bilgi için lütfen  [Windows 10 sürüm 2004 bilinen sorunlar](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="bf597-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>