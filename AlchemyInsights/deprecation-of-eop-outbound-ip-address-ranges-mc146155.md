---
title: 1065 EOP giden IP adresi aralıklarının amortismanı MC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704617"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="05ebb-102">EOP giden IP adres aralıklarının amortismanı</span><span class="sxs-lookup"><span data-stu-id="05ebb-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="05ebb-103">Kuruluşunuzla ilgili olası bir sorun tespit ettik ve (26 Ekim 2018'e kadar düzeltilmezse) şirket içi veya harici hedeflerinize posta akışını kırabilir.</span><span class="sxs-lookup"><span data-stu-id="05ebb-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="05ebb-104">Daha önce de belirtildiği gibi, IP adresi aralığı yönetimini basitleştirmek için, Microsoft 365 dışında e-posta gönderip almak için kullanılan Exchange Çevrimiçi Koruma (EOP) IP adresi aralıklarını birleştiririz.</span><span class="sxs-lookup"><span data-stu-id="05ebb-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="05ebb-105">Analizlerimiz, posta akışı bağlayıcılarında yapılandırdığınız harici e-posta kaynaklarından veya hedeflerinden birinin veya birkaçının [burada](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)gösterilen IP adresi aralıklarından bağlantıları kabul etmediğini gösterir.</span><span class="sxs-lookup"><span data-stu-id="05ebb-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="05ebb-106">Bu kaynakların ve destinasyonların yayınlanmış tüm [EOP IP adreslerine](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)ve bağlantılarını kabul etmesini sağlamak için 26 Ekim'den önce harekete geçin.</span><span class="sxs-lookup"><span data-stu-id="05ebb-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="05ebb-107">Bu değişiklik hakkında daha fazla bilgi için lütfen Mesaj Merkezi gönderilerine [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)veya [MC149274'e](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)bakın.</span><span class="sxs-lookup"><span data-stu-id="05ebb-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="05ebb-108">**Not**: Son nokta güncelleştirmeleri için HTML, XML ve RSS üzerinden daha önce IP veya URL yayımlama kullandıysanız, bu tür güncelleştirmeleri otomatikleştirmek için yeni web hizmetlerine de geçiş yapmalısınız.</span><span class="sxs-lookup"><span data-stu-id="05ebb-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="05ebb-109">Daha fazla bilgi için Microsoft [365 uç nokta kategorisi ve Microsoft 365 IP Adresi ve URL web hizmetine](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)bakın.</span><span class="sxs-lookup"><span data-stu-id="05ebb-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
