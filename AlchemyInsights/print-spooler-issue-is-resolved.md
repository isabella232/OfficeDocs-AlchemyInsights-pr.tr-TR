---
title: Yazdırma biriktirme sorunu çözüldü
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088528"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="b9979-102">Yazdırma biriktirme sorunu çözüldü</span><span class="sxs-lookup"><span data-stu-id="b9979-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="b9979-103">Aygıtınız Windows 10 **İşletim Sistemi Build 19041.329**ile güncelleştirildiyse, belirli yazıcıların yazdırılamadığı bir sorunu gözlemlemiş olabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b9979-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="b9979-104">Yazdırma makinacısı yazdırmaya çalışırken beklenmedik bir şekilde hata yapabilir veya kapanabilir ve etkilenen yazıcıdan çıkış gelmez.</span><span class="sxs-lookup"><span data-stu-id="b9979-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="b9979-105">Bu sorun OS Build **19041.331,** [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)olarak çözülür.</span><span class="sxs-lookup"><span data-stu-id="b9979-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="b9979-106">**Devam eden soruşturma**</span><span class="sxs-lookup"><span data-stu-id="b9979-106">**Ongoing investigation**</span></span>

<span data-ttu-id="b9979-107">Yerel Güvenlik Otoritesi Alt Sistem Servisi (LSASS) dosyası\*\* (Isass.exe) \*\*hata mesajı ile bazı cihazlarda başarısız olabilir, "Kritik bir sistem süreci, C:\WINDOWS\system32\Isass.exe, durum kodu c0000008 ile başarısız oldu.</span><span class="sxs-lookup"><span data-stu-id="b9979-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="b9979-108">Makine nin yeniden başlatılması gerekiyor" dedi.</span><span class="sxs-lookup"><span data-stu-id="b9979-108">The machine must now be restarted".</span></span>  <span data-ttu-id="b9979-109">**Microsoft bir çözüm üzerinde çalışıyor ve yaklaşan bir sürümde bir güncelleştirme sağlayacaktır.**</span><span class="sxs-lookup"><span data-stu-id="b9979-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="b9979-110">Daha fazla bilgi için lütfen [Windows 10 Sürüm 2004'ün bilinen sorunlarına](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)göz atın.</span><span class="sxs-lookup"><span data-stu-id="b9979-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>