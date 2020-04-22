---
title: SpamHaus tarafından engellenen e-posta gönderme hatası
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714278"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="cde00-102">E-posta gönderme hatası: İstemci ana bilgisayar Spamhaus kullanılarak engellendi</span><span class="sxs-lookup"><span data-stu-id="cde00-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="cde00-103">İletiyi gönderen IP adresi [Spamhaus'a](https://go.microsoft.com/fwlink/p/?linkid=123245)ait bir blok listesindedir.</span><span class="sxs-lookup"><span data-stu-id="cde00-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="cde00-104">Spamhaus tarafından engellenmesinin nedenleri arasında, gizliliği ihlal edilen hesaplar, genel BIR IP adresini paylaşan tehlikeye atılmış makineler ve Internet Servis Sağlayıcısı (ISS) ilkeleri yer almaktadır.</span><span class="sxs-lookup"><span data-stu-id="cde00-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="cde00-105">Olası düzeltmeler şunlardır:</span><span class="sxs-lookup"><span data-stu-id="cde00-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="cde00-106">Kaynak e-posta sunucusunu kontrol ettiğiniz engellenen gelen iletiler için nedenini belirlemeniz ve engellemeyi Spamhaus web sitesinden kaldırmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="cde00-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="cde00-107">Kaynak IP adresinin başka birine ait olduğu engellenen gelen iletiler için adres sahibinin engellemeyi Spamhaus web sitesinden kaldırması gerekir.</span><span class="sxs-lookup"><span data-stu-id="cde00-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="cde00-108">IP adresi İlke Blok Listesi'nde (PBL) yer alıyorsa, sahibi farklı bir statik IP adresi atayabilir veya adresi PBL'den kaldırabilir.</span><span class="sxs-lookup"><span data-stu-id="cde00-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="cde00-109">Microsoft'a bağlı etki alanınızdan engellenen giden iletiler için, iletiler üçüncü taraf hizmeti aracılığıyla yönlendirilirse bu hatayı alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cde00-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="cde00-110">Engellenen IP adresi sahibini bulmak için bir WHOIS arama aracı kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cde00-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
