---
title: Office uygulamalarını düzeltmeÜzgünüz, geçici sunucu sorunları iletisi alıyoruz
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
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764137"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="5ed36-102">Office uygulamalarını düzeltme "Üzgünüz, geçici sunucu sorunları yaşıyoruz" iletisi</span><span class="sxs-lookup"><span data-stu-id="5ed36-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="5ed36-103">Bu iletiyi alırsanız, aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="5ed36-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="5ed36-104">Office uygulamalarına Internet erişimini engellemediklerini doğrulamak için güvenlik duvarınızı, virüsten koruma yazılımınızı ve proxy ayarlarınızı kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="5ed36-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="5ed36-105">[URL'lere ve IP adres aralıklarına](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)bakın.</span><span class="sxs-lookup"><span data-stu-id="5ed36-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="5ed36-106">**Başlat** > **Çalıştır'a**gidin ve ardından **services.msc**yazın.</span><span class="sxs-lookup"><span data-stu-id="5ed36-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="5ed36-107">Aşağıdaki hizmetlerin tümlerinin çalıştığını unutmayın:</span><span class="sxs-lookup"><span data-stu-id="5ed36-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="5ed36-108">Ağa Bağlı Cihazlar Otomatik Kurulum</span><span class="sxs-lookup"><span data-stu-id="5ed36-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="5ed36-109">Ağ Listesi Hizmeti</span><span class="sxs-lookup"><span data-stu-id="5ed36-109">Network List Service</span></span>
    - <span data-ttu-id="5ed36-110">Ağ Konum Farkındalığı</span><span class="sxs-lookup"><span data-stu-id="5ed36-110">Network Location Awareness</span></span>
    - <span data-ttu-id="5ed36-111">Windows Etkinlik Günlüğü</span><span class="sxs-lookup"><span data-stu-id="5ed36-111">Windows Event Log</span></span>

<span data-ttu-id="5ed36-112">Bu hizmetlerden biri çalışmıyorsa, başlatmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="5ed36-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="5ed36-113">Hizmeti başlatmakta sorun varsa, yüksek izinleri olan bir komut istemi açarak aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="5ed36-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="5ed36-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="5ed36-114">**sfc /scannow**</span></span>

<span data-ttu-id="5ed36-115">Bu komut bittikten sonra bilgisayarı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="5ed36-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="5ed36-116">Ayrıntılı bilgi için [bkz: "Üzgünüz, hesabınıza bağlanabiliyoruz. Lütfen daha sonra tekrar deneyin" hatanızı etkinleştirdiğinizde.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="5ed36-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>