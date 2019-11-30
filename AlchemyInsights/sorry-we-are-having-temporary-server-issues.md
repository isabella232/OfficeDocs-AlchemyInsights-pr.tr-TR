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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628010"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="aaf76-102">Office uygulamalarını düzeltme "Üzgünüz, geçici sunucu sorunları yaşıyoruz" iletisi</span><span class="sxs-lookup"><span data-stu-id="aaf76-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="aaf76-103">Bu iletiyi alırsanız, aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="aaf76-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="aaf76-104">Office uygulamalarına Internet erişimini engellemediklerini doğrulamak için güvenlik duvarınızı, virüsten koruma yazılımınızı ve proxy ayarlarınızı kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="aaf76-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="aaf76-105">Bkz. [Office 365 URL'leri ve IP adresi aralıkları.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="aaf76-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="aaf76-106">**Başlat** > **Çalıştır'a**gidin ve ardından **services.msc**yazın.</span><span class="sxs-lookup"><span data-stu-id="aaf76-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="aaf76-107">Aşağıdaki hizmetlerin tümlerinin çalıştığını unutmayın:</span><span class="sxs-lookup"><span data-stu-id="aaf76-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="aaf76-108">Ağa Bağlı Cihazlar Otomatik Kurulum</span><span class="sxs-lookup"><span data-stu-id="aaf76-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="aaf76-109">Ağ Listesi Hizmeti</span><span class="sxs-lookup"><span data-stu-id="aaf76-109">Network List Service</span></span>
    - <span data-ttu-id="aaf76-110">Ağ Konum Farkındalığı</span><span class="sxs-lookup"><span data-stu-id="aaf76-110">Network Location Awareness</span></span>
    - <span data-ttu-id="aaf76-111">Windows Etkinlik Günlüğü</span><span class="sxs-lookup"><span data-stu-id="aaf76-111">Windows Event Log</span></span>

<span data-ttu-id="aaf76-112">Bu hizmetlerden biri çalışmıyorsa, başlatmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="aaf76-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="aaf76-113">Hizmeti başlatmakta sorun varsa, yüksek izinleri olan bir komut istemi açarak aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="aaf76-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="aaf76-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="aaf76-114">**sfc /scannow**</span></span>

<span data-ttu-id="aaf76-115">Bu komut bittikten sonra bilgisayarı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="aaf76-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="aaf76-116">Ayrıntılı bilgi için [bkz: "Üzgünüz, hesabınıza bağlanabiliyoruz. Office 365'ten Office'i etkinleştirdiğinizde lütfen daha sonra tekrar deneyin" hatası.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="aaf76-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>