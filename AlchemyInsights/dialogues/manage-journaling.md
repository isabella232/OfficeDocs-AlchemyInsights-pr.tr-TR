---
title: Günlüğü yönetme
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527460"
---
# <a name="manage-journaling"></a><span data-ttu-id="a2299-102">Günlüğü yönetme</span><span class="sxs-lookup"><span data-stu-id="a2299-102">Manage journaling</span></span>

<span data-ttu-id="a2299-103">Günlük kaydı, gelen ve giden e-posta iletişimlerini kaydederek, kuruma yasal, yasal ve kurumsal uyumluluk gereksinimlerini yanıtlamada yardımcı olabilir.</span><span class="sxs-lookup"><span data-stu-id="a2299-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="a2299-104">Şunları unutmayın:</span><span class="sxs-lookup"><span data-stu-id="a2299-104">Keep in mind:</span></span>

* <span data-ttu-id="a2299-105">Günlüğü [yönetemeden önce Kuruluş](https://go.microsoft.com/fwlink/?linkid=2115259) Yönetimi [ve](https://go.microsoft.com/fwlink/?linkid=2115469) Kayıt Yönetimi izinlerine sahip olmak gerekir.</span><span class="sxs-lookup"><span data-stu-id="a2299-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="a2299-106">Bir günlük posta kutunuz ve (isteğe bağlı olarak) yapılandırılmış alternatif bir günlük posta kutunuz gerekir.</span><span class="sxs-lookup"><span data-stu-id="a2299-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="a2299-107">Daha fazla bilgi edinmek için, [Exchange Online'da Günlüğü Yapılandırma'ya bakın.](https://go.microsoft.com/fwlink/?linkid=2115260)</span><span class="sxs-lookup"><span data-stu-id="a2299-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="a2299-108">Exchange Online'da, oluşturabilirsiniz günlük kuralları sayısının bir sınırı vardır.</span><span class="sxs-lookup"><span data-stu-id="a2299-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="a2299-109">Ayrıntılar için [Günlük, aktarım ve gelen kutusu kuralı sınırlarına bakın.](https://go.microsoft.com/fwlink/?linkid=2115261)</span><span class="sxs-lookup"><span data-stu-id="a2299-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="a2299-110">Exchange Online, bir Exchange Online posta kutusuna günlük raporları teslimi desteklemez.</span><span class="sxs-lookup"><span data-stu-id="a2299-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="a2299-111">Şirket içi arşivleme sisteminin veya üçüncü taraf arşivleme hizmetinin e-posta adresini günlük posta kutusu olarak belirtebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a2299-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
