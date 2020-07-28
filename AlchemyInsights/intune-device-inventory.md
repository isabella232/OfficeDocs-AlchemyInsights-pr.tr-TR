---
title: Intune Cihaz Envanteri
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440480"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="01273-102">Intune Cihaz Envanteri</span><span class="sxs-lookup"><span data-stu-id="01273-102">Intune Device Inventory</span></span>

<span data-ttu-id="01273-103">Cihazlar bıçağı, intune'da yönetim altındaki aygıtlar için yönetici içgörüsü sağlar.</span><span class="sxs-lookup"><span data-stu-id="01273-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="01273-104">Gösterilen bilgiler şunları içerir: Donanım, Keşfedilen uygulamalar, Aygıt Uyumluluğu durumu ve Aygıt Yapılandırma durumu.</span><span class="sxs-lookup"><span data-stu-id="01273-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="01273-105">Donanım ve keşfedilen uygulamalar için envanter verileri yedi günlük bir döngüde toplanır.</span><span class="sxs-lookup"><span data-stu-id="01273-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="01273-106">Bildirilen uygulamaların ve bildirilen donanımın belirli öğeleri, aygıt işletim sistemine ve cihazın kişisel veya kurumsal sahip olup olmadığına bağlı olarak farklılık gösterir.</span><span class="sxs-lookup"><span data-stu-id="01273-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="01273-107">Daha fazla bilgi için Bkz. [Intune'daki cihaz ayrıntılarını görün.](https://docs.microsoft.com/intune/device-inventory)</span><span class="sxs-lookup"><span data-stu-id="01273-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="01273-108">**SSS**</span><span class="sxs-lookup"><span data-stu-id="01273-108">**FAQ**</span></span>

<span data-ttu-id="01273-109">S: Intune kayıtlı Windows aygıtlarında bulunan uygulamaların tam bir envanter listesini almıyorum.</span><span class="sxs-lookup"><span data-stu-id="01273-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="01273-110">Neden olmasın?</span><span class="sxs-lookup"><span data-stu-id="01273-110">Why not?</span></span>

<span data-ttu-id="01273-111">C: Şu anda, yalnızca modern uygulamalar kurumsal aygıtlar olarak tanımlanan Windows 10 bilgisayarları için listelenmiştir.</span><span class="sxs-lookup"><span data-stu-id="01273-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="01273-112">Intune, bu cihazlarda yüklü olan Win32 uygulamaları hakkında bilgi toplamaz.</span><span class="sxs-lookup"><span data-stu-id="01273-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="01273-113">S: Telefon numaraları neden tüm cihazlardan toplanmaz?</span><span class="sxs-lookup"><span data-stu-id="01273-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="01273-114">C: Intune'da kurumsal aygıt olarak sınıflandırılan telefonlar, örneğin bir mobil cihaz envanter raporu çalıştırdığınızda tam telefon numarasıyla tanımlanmaz.</span><span class="sxs-lookup"><span data-stu-id="01273-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="01273-115">Bring-you-own-kendi cihaz telefon numaraları her zaman kısmen yıldız işaretleri (\*\*\*\*) ile maskeli ve yalnızca son dört basamak gösterir.</span><span class="sxs-lookup"><span data-stu-id="01273-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>