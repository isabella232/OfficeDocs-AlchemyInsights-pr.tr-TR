---
title: Etkinleştirme sorunu-şu an bağlantı kuramıyoruz
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726003"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="41d0b-102">Microsoft 365 uygulamalarını düzeltme "hemen bağlantı kuramıyoruz" iletisi</span><span class="sxs-lookup"><span data-stu-id="41d0b-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="41d0b-103">Bu iletiyi alırsanız, aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="41d0b-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="41d0b-104">Güvenlik duvarınızın, virüsten koruma yazılımınızın ve proxy ayarlarınızın Internet erişimini Microsoft 365 uygulamalarına engellemediğinden emin olmak için denetleyin.</span><span class="sxs-lookup"><span data-stu-id="41d0b-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="41d0b-105">[Microsoft URL 'leri ve IP adresi aralıklarını](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)görün.</span><span class="sxs-lookup"><span data-stu-id="41d0b-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="41d0b-106">Başlat 'ı **başlatın**  >  **Run**ve ardından **Services. msc**yazın.</span><span class="sxs-lookup"><span data-stu-id="41d0b-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="41d0b-107">Aşağıdaki hizmetlerin tümünün çalıştığından emin olun:</span><span class="sxs-lookup"><span data-stu-id="41d0b-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="41d0b-108">Ağ bağlantılı cihazların otomatik kurulumu</span><span class="sxs-lookup"><span data-stu-id="41d0b-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="41d0b-109">Ağ listesi hizmeti</span><span class="sxs-lookup"><span data-stu-id="41d0b-109">Network List Service</span></span>
    - <span data-ttu-id="41d0b-110">Ağ konumu tanıma</span><span class="sxs-lookup"><span data-stu-id="41d0b-110">Network Location Awareness</span></span>
    - <span data-ttu-id="41d0b-111">Windows olay günlüğü</span><span class="sxs-lookup"><span data-stu-id="41d0b-111">Windows Event Log</span></span>

<span data-ttu-id="41d0b-112">Bu hizmetlerden biri çalışmıyorsa, başlatmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="41d0b-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="41d0b-113">Hizmeti başlatırken bir sorun yaşıyorsanız, yükseltilmiş izinlerle komut istemini açarak aşağıdaki komutu çalıştırabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="41d0b-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="41d0b-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="41d0b-114">**sfc /scannow**</span></span>

<span data-ttu-id="41d0b-115">Bu komut bittiğinde bilgisayarı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="41d0b-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="41d0b-116">Ayrıntılı bilgi için, [hesabınıza bağlanamıyoruz "Üzgünüz. Office 'i Microsoft 365 'i etkinleştirdiğinizde lütfen daha sonra tekrar deneyin](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="41d0b-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>