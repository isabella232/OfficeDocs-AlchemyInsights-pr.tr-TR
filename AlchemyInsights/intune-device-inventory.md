---
title: Intune cihaz stoğu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667898"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="6250b-102">Intune cihaz stoğu</span><span class="sxs-lookup"><span data-stu-id="6250b-102">Intune Device Inventory</span></span>

<span data-ttu-id="6250b-103">Cihazlar Blade, cihaz temelinde, Intune 'da yönetim 'in altındaki aygıtlara fikir sağlar.</span><span class="sxs-lookup"><span data-stu-id="6250b-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="6250b-104">Gösterilen bilgiler: donanım, bulunan uygulamalar, cihaz uyumluluk durumu ve cihaz yapılandırma durumu.</span><span class="sxs-lookup"><span data-stu-id="6250b-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="6250b-105">Donanım için envanter verileri ve bulunan uygulamalar, yedi günlük döngüde toplanır.</span><span class="sxs-lookup"><span data-stu-id="6250b-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="6250b-106">Uygulamalar ve belirli donanım öğeleri, cihaz işletim sistemine bağlı olarak ve cihazın kişisel veya şirket sahibi olup olmadığı fark edilir.</span><span class="sxs-lookup"><span data-stu-id="6250b-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="6250b-107">Daha fazla bilgi için bkz [.](https://docs.microsoft.com/intune/device-inventory)</span><span class="sxs-lookup"><span data-stu-id="6250b-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="6250b-108">**SSS**</span><span class="sxs-lookup"><span data-stu-id="6250b-108">**FAQ**</span></span>

<span data-ttu-id="6250b-109">S: Intune kayıtlı Windows cihazlarında tüm uygulamaların tam envanter listesini almıyorum.</span><span class="sxs-lookup"><span data-stu-id="6250b-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="6250b-110">Neden olmasın?</span><span class="sxs-lookup"><span data-stu-id="6250b-110">Why not?</span></span>

<span data-ttu-id="6250b-111">A: Şu anda yalnızca modern uygulamalar, kurumsal cihazlar olarak tanımlanan Windows 10 bilgisayarlarında listelenir.</span><span class="sxs-lookup"><span data-stu-id="6250b-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="6250b-112">Intune, bu cihazlarda yüklü Win32 uygulamaları hakkında bilgi toplamaz.</span><span class="sxs-lookup"><span data-stu-id="6250b-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="6250b-113">S: telefon numaraları neden tüm cihazlardan toplanmadı?</span><span class="sxs-lookup"><span data-stu-id="6250b-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="6250b-114">A: Örneğin, bir mobil cihaz envanter raporu çalıştırırsanız, Intune 'da şirket cihazları olarak kategorilere ayrılan telefonlar tam telefon numarasıyla tanımlanmayabilir.</span><span class="sxs-lookup"><span data-stu-id="6250b-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="6250b-115">Yanınızda getirin-kendi-cihaz telefon numaraları her zaman yıldız işareti (\* \* \* \*) ile kısmen maskelenir ve yalnızca son dört basamağı gösterir.</span><span class="sxs-lookup"><span data-stu-id="6250b-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>