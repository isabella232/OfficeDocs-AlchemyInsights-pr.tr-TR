---
title: Giden geçiş havuzu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381866"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="9384d-102">Giden geçiş havuzu</span><span class="sxs-lookup"><span data-stu-id="9384d-102">Outbound relay pool</span></span>

<span data-ttu-id="9384d-103">Microsoft, e-postanın geçiş ve iletme için yapılandırmasında değişiklikler Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9384d-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="9384d-104">Bazı senaryolarda iletiler, özel bir geçiş havuzu kullanılarak Microsoft 365 bir havuz kullanılarak ilet ister başka bir kullanıcıya iletebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9384d-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="9384d-105">Geçiş havuzu kullanılarak gönderilen iletiler alıcının gereksiz posta klasörüne kadar olabilir.</span><span class="sxs-lookup"><span data-stu-id="9384d-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="9384d-106">Daha fazla bilgi için [bkz. Giden teslim havuzları](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="9384d-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="9384d-107">Geçiş havuzunun kullanımıyla ilgili bir senaryodan kaçınmak için, iletili/geçişli iletilerin aşağıdaki ölçütlerden birini karşılaması gerekir:</span><span class="sxs-lookup"><span data-stu-id="9384d-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="9384d-108">Giden gönderen, kiracının kabul edilen etki alanıdır.</span><span class="sxs-lookup"><span data-stu-id="9384d-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="9384d-109">İleti ilk kez geldiğinde Sender Policy Framework (SPF) Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9384d-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="9384d-110">P2 gönderen etki alanındaki DomainKeys Identified Mail (DKIM), ileti gönderene geldiğinde Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9384d-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="9384d-111">Yukarıdaki ölçütlere uyan iletiler geçiş havuzundan aktarlanmaz.</span><span class="sxs-lookup"><span data-stu-id="9384d-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="9384d-112">Etki alanınıza yönelik MX kaydı üçüncü taraf veya şirket içi bir sunucuya işaret ediyorsa, SPF doğrulamanın gelen e-posta için doğru olduğundan ve geçiş havuzu üzerinden e-posta gönderilmesini önlemek için gelişmiş filtrelemeyi kullanın.</span><span class="sxs-lookup"><span data-stu-id="9384d-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="9384d-113">**Geçiş havuzunun etkilenmesi ile ilgili durumu nasıl anlarız?**</span><span class="sxs-lookup"><span data-stu-id="9384d-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="9384d-114">İletili veya geçişli e-postanız yukarıdaki ölçütlerden birini kullanıyorsa, iletiler geçiş havuzundan aktarıilir.</span><span class="sxs-lookup"><span data-stu-id="9384d-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="9384d-115">Öte yandan, ileti bir geçiş havuzu aracılığıyla gönderilirse, giden sunucu IP'si 40.95.0.0/16 aralığındadır ve giden sunucu adı **rly** içerir.</span><span class="sxs-lookup"><span data-stu-id="9384d-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

