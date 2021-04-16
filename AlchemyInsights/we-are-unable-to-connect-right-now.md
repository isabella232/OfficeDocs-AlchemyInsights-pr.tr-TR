---
title: Etkinleştirme Sorunu - Şu anda bağlanaayız
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
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806462"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="2ec19-102">Microsoft 365 uygulamalarını düzeltme "Şu anda bağlanalarız" iletisi</span><span class="sxs-lookup"><span data-stu-id="2ec19-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="2ec19-103">Bu iletiyi alırsanız, şunları deneyin:</span><span class="sxs-lookup"><span data-stu-id="2ec19-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="2ec19-104">Güvenlik duvarınızı, virüsten koruma yazılımınızı ve proxy ayarlarınızı kontrol edin ve Microsoft 365 uygulamalarına İnternet erişimini engellemelerini engellemez.</span><span class="sxs-lookup"><span data-stu-id="2ec19-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="2ec19-105">Bkz. [Microsoft URL'leri ve IP adresi aralıkları.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="2ec19-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="2ec19-106">Başlangıç **Çalıştırma'ya**  >  **gidin** ve **services.msc yazın.**</span><span class="sxs-lookup"><span data-stu-id="2ec19-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="2ec19-107">Aşağıdaki hizmetlerin hepsinin çalıştırlı olduğundan emin olun:</span><span class="sxs-lookup"><span data-stu-id="2ec19-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="2ec19-108">Ağ Bağlantılı Cihazlar Otomatik Kurulumu</span><span class="sxs-lookup"><span data-stu-id="2ec19-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="2ec19-109">Ağ Listesi Hizmeti</span><span class="sxs-lookup"><span data-stu-id="2ec19-109">Network List Service</span></span>
    - <span data-ttu-id="2ec19-110">Ağ Konumu Farkındalığı</span><span class="sxs-lookup"><span data-stu-id="2ec19-110">Network Location Awareness</span></span>
    - <span data-ttu-id="2ec19-111">Windows Olay Günlüğü</span><span class="sxs-lookup"><span data-stu-id="2ec19-111">Windows Event Log</span></span>

<span data-ttu-id="2ec19-112">Bu hizmetlerden biri çalışmıyorsa, başlatmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="2ec19-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="2ec19-113">Hizmeti başlatmayla ilgili bir sorun varsa yükseltilmiş izinlerle bir komut istemi açarak aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="2ec19-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="2ec19-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="2ec19-114">**sfc /scannow**</span></span>

<span data-ttu-id="2ec19-115">Bu komut tamamdikten sonra bilgisayarı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="2ec19-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="2ec19-116">Ayrıntılı bilgi için [bkz. "Ne üzgünüz, hesabınıza bağlana üzgünüz. Office'i Microsoft 365'den etkinleştirirken lütfen daha sonra yeniden deneyin" hatası.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="2ec19-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>