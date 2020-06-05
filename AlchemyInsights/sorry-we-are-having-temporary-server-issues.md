---
title: Microsoft 365 uygulamaları sabitleme Üzgünüz, biz geçici sunucu sorunları mesajı yaşıyorsanız
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582723"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="d721c-102">Microsoft 365 uygulamalarını düzeltme "Üzgünüz, geçici sunucu sorunları yaşıyoruz" iletisi</span><span class="sxs-lookup"><span data-stu-id="d721c-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="d721c-103">Bu iletiyi alırsanız, aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="d721c-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="d721c-104">Microsoft 365 uygulamalarına Internet erişimini engellemediklerini doğrulamak için güvenlik duvarınızı, virüsten koruma yazılımınızı ve proxy ayarlarınızı kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="d721c-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="d721c-105">[URL'lere ve IP adres aralıklarına](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)bakın.</span><span class="sxs-lookup"><span data-stu-id="d721c-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="d721c-106">Başlat **Start**  >  **Çalıştır'a**gidin ve ardından **services.msc**yazın.</span><span class="sxs-lookup"><span data-stu-id="d721c-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="d721c-107">Aşağıdaki hizmetlerin tümlerinin çalıştığını unutmayın:</span><span class="sxs-lookup"><span data-stu-id="d721c-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="d721c-108">Ağa Bağlı Cihazlar Otomatik Kurulum</span><span class="sxs-lookup"><span data-stu-id="d721c-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="d721c-109">Ağ Listesi Hizmeti</span><span class="sxs-lookup"><span data-stu-id="d721c-109">Network List Service</span></span>
    - <span data-ttu-id="d721c-110">Ağ Konum Farkındalığı</span><span class="sxs-lookup"><span data-stu-id="d721c-110">Network Location Awareness</span></span>
    - <span data-ttu-id="d721c-111">Windows Etkinlik Günlüğü</span><span class="sxs-lookup"><span data-stu-id="d721c-111">Windows Event Log</span></span>

<span data-ttu-id="d721c-112">Bu hizmetlerden biri çalışmıyorsa, başlatmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="d721c-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="d721c-113">Hizmeti başlatmakta sorun varsa, yüksek izinleri olan bir komut istemi açarak aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="d721c-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="d721c-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="d721c-114">**sfc /scannow**</span></span>

<span data-ttu-id="d721c-115">Bu komut bittikten sonra bilgisayarı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="d721c-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="d721c-116">Ayrıntılı bilgi için [bkz: "Üzgünüz, hesabınıza bağlanabiliyoruz. Lütfen daha sonra tekrar deneyin" hatanızı etkinleştirdiğinizde.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="d721c-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>