---
title: Etkinleştirme Sorunu - Şu anda bağlanamıyoruz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716192"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="a284d-102">Office uygulamalarını düzeltme "Şu anda bağlanamıyoruz" iletisi</span><span class="sxs-lookup"><span data-stu-id="a284d-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="a284d-103">Bu iletiyi alırsanız, aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="a284d-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="a284d-104">Office uygulamalarına Internet erişimini engellemediklerini doğrulamak için güvenlik duvarınızı, virüsten koruma yazılımınızı ve proxy ayarlarınızı kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="a284d-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="a284d-105">[Bkz. Microsoft URL'leri ve IP adresi aralıkları.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="a284d-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="a284d-106">**Başlat** > **Çalıştır'a**gidin ve ardından **services.msc**yazın.</span><span class="sxs-lookup"><span data-stu-id="a284d-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="a284d-107">Aşağıdaki hizmetlerin tümlerinin çalıştığını unutmayın:</span><span class="sxs-lookup"><span data-stu-id="a284d-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="a284d-108">Ağa Bağlı Cihazlar Otomatik Kurulum</span><span class="sxs-lookup"><span data-stu-id="a284d-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="a284d-109">Ağ Listesi Hizmeti</span><span class="sxs-lookup"><span data-stu-id="a284d-109">Network List Service</span></span>
    - <span data-ttu-id="a284d-110">Ağ Konum Farkındalığı</span><span class="sxs-lookup"><span data-stu-id="a284d-110">Network Location Awareness</span></span>
    - <span data-ttu-id="a284d-111">Windows Etkinlik Günlüğü</span><span class="sxs-lookup"><span data-stu-id="a284d-111">Windows Event Log</span></span>

<span data-ttu-id="a284d-112">Bu hizmetlerden biri çalışmıyorsa, başlatmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="a284d-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="a284d-113">Hizmeti başlatmakta sorun varsa, yüksek izinleri olan bir komut istemi açarak aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="a284d-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="a284d-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="a284d-114">**sfc /scannow**</span></span>

<span data-ttu-id="a284d-115">Bu komut bittikten sonra bilgisayarı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="a284d-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="a284d-116">Ayrıntılı bilgi için [bkz: "Üzgünüz, hesabınıza bağlanabiliyoruz. Microsoft 365'ten Office'i etkinleştirdiğinizde lütfen daha sonra tekrar deneyin" hatası.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="a284d-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>