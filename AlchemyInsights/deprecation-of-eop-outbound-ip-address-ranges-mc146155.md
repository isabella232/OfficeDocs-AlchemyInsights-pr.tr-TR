---
title: 1065 EOP giden IP adresi rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806815"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="7e987-102">Giden IP adresi aralıklarının kullanımdan kaldırılması</span><span class="sxs-lookup"><span data-stu-id="7e987-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="7e987-103">Kuruluşunuzda (Ekim 26 ' ya kadar düzeltilmez, 2018) Şirket içi veya dış hedeflerine posta akışını bozabilecek olası bir sorun algıladık.</span><span class="sxs-lookup"><span data-stu-id="7e987-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="7e987-104">Daha önce, IP adres aralığı yönetimini basitleştirmek amacıyla, Microsoft 365 dışında e-posta göndermek ve almak için kullanılan Exchange Online Protection (EOP) IP adresi aralıklarını birleştiriyoruz.</span><span class="sxs-lookup"><span data-stu-id="7e987-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="7e987-105">Çözümümüz, posta akışı bağlayıcılarının, [burada](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)gösterilen IP adresi aralıklarından gelen bağlantıları kabul etmediği anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="7e987-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="7e987-106">Bu kaynakların ve hedeflerin tüm [yayımlanan EOP IP adreslerine](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)yönelik bağlantıları kabul edeceği Için, Ekim 26 ' dan önce hareket edin.</span><span class="sxs-lookup"><span data-stu-id="7e987-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="7e987-107">Bu değişiklik hakkında daha fazla bilgi için bkz: Message Center gönderileri [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)veya [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="7e987-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="7e987-108">**Not**: daha önce HTML, XML ve RSS aracılığıyla uç nokta güncelleştirmelerinde IP veya URL yayımlamayı kullandıysanız, bu tür güncellemeleri otomatikleştirmek için yeni Web hizmetlerine de geçiş yapmalısınız.</span><span class="sxs-lookup"><span data-stu-id="7e987-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="7e987-109">Daha fazla bilgi için bkz: [microsoft 365 uç nokta kategorileri ve microsoft 365 IP adresi ve URL Web hizmeti](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="7e987-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
