---
title: Linux'ta Uç Nokta için Microsoft Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11490"
- "9001464"
ms.openlocfilehash: 99894d83c51e11ea6dd1746568762eac856306b3
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731976"
---
# <a name="microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="b4d84-102">Linux'ta Uç Nokta için Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="b4d84-102">Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="b4d84-103">Ayrıntılı Linux belgeleri için bkz. [Linux'ta Uç Nokta için Microsoft Defender](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux).</span><span class="sxs-lookup"><span data-stu-id="b4d84-103">For detailed Linux documentation, see [Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux).</span></span>

<span data-ttu-id="b4d84-104">Sistem ve yükleme bilgileri için bkz:</span><span class="sxs-lookup"><span data-stu-id="b4d84-104">For system and installation information, see:</span></span>

- [<span data-ttu-id="b4d84-105">Önkoşullar</span><span class="sxs-lookup"><span data-stu-id="b4d84-105">Prerequisites</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#prerequisites)
- [<span data-ttu-id="b4d84-106">Sistem gereksinimleri</span><span class="sxs-lookup"><span data-stu-id="b4d84-106">System requirements</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#system-requirements)
- [<span data-ttu-id="b4d84-107">Yükleme yönergeleri</span><span class="sxs-lookup"><span data-stu-id="b4d84-107">Installation instructions</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#installation-instructions)
- [<span data-ttu-id="b4d84-108">Ağ bağlantıları</span><span class="sxs-lookup"><span data-stu-id="b4d84-108">Network connections</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#network-connections)

<span data-ttu-id="b4d84-109">Yönergeler için bkz:</span><span class="sxs-lookup"><span data-stu-id="b4d84-109">For instructions, see:</span></span>

- [<span data-ttu-id="b4d84-110">Cihaz ara sunucusunu ve İnternet bağlantısı ayarlarını yapılandırma</span><span class="sxs-lookup"><span data-stu-id="b4d84-110">Configure device proxy and Internet connectivity settings</span></span>](/microsoft-365/security/defender-endpoint/configure-proxy-internet#enable-access-to-microsoft-defender-atp-service-urls-in-the-proxy-server)
- [<span data-ttu-id="b4d84-111">Linux'ta Uç Nokta için Microsoft Defender güncelleştirmelerini dağıtma</span><span class="sxs-lookup"><span data-stu-id="b4d84-111">Deploy updates for Microsoft Defender for Endpoint on Linux</span></span>](/microsoft-365/security/defender-endpoint/linux-updates)
- [<span data-ttu-id="b4d84-112">Linux'ta Uç Nokta için Microsoft Defender nasıl yapılandırılır</span><span class="sxs-lookup"><span data-stu-id="b4d84-112">How to configure Microsoft Defender for Endpoint on Linux</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#how-to-configure-microsoft-defender-for-endpoint-on-linux)
- [<span data-ttu-id="b4d84-113">Desteklenen komutlar</span><span class="sxs-lookup"><span data-stu-id="b4d84-113">Supported commands</span></span>](/microsoft-365/security/defender-endpoint/linux-resources#supported-commands)

## <a name="i-need-help"></a><span data-ttu-id="b4d84-114">Yardıma ihtiyacım var!</span><span class="sxs-lookup"><span data-stu-id="b4d84-114">I need help!</span></span>

<span data-ttu-id="b4d84-115">Bulmakta olmadığınız bilgileri/yardımı bulamazsanız, arama dizenizi daraltyın.</span><span class="sxs-lookup"><span data-stu-id="b4d84-115">If you can't find the information/help you're looking for, refine your search string.</span></span>

<span data-ttu-id="b4d84-116">Microsoft Desteği'ne başvurmadan önce, sorunlarınızı araştırmanız için gereken verileri toplamayı ve bunu bilete iliştirin.</span><span class="sxs-lookup"><span data-stu-id="b4d84-116">Before contacting Microsoft Support, make sure to collect the data required to investigate your issue, and attach it to the ticket.</span></span> <span data-ttu-id="b4d84-117">Tanılama bilgilerini toplama adımları için bkz. Tanılama [verilerini toplama](/microsoft-365/security/defender-endpoint/linux-resources#collect-diagnostic-information).</span><span class="sxs-lookup"><span data-stu-id="b4d84-117">For steps to collect the diagnosic information, see [Collect diagnostic data](/microsoft-365/security/defender-endpoint/linux-resources#collect-diagnostic-information).</span></span>