---
title: SpamHaus tarafından engellenen e-posta gönderme hatası
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813744"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="53282-102">E-posta gönderme hatası: İstemci ana bilgisayarı Spamhaus kullanılarak engellendi</span><span class="sxs-lookup"><span data-stu-id="53282-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="53282-103">İletiyi gönderen IP adresi Spamhaus'un engellenenler [listesinde yer alıyor.](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="53282-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="53282-104">Güvenliği tehlikeye atılmış hesaplar, ortak IP adresini paylaşarak güvenliği tehlikeye makineler ve İnternet Servis Sağlayıcısı (ISS) ilkeleri Spamhaus'un engelleme nedenlerinden bazılarıdır.</span><span class="sxs-lookup"><span data-stu-id="53282-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="53282-105">Olası düzeltmeler:</span><span class="sxs-lookup"><span data-stu-id="53282-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="53282-106">Kaynak e-posta sunucusunu kontrol etmek istediğiniz engellenen gelen iletiler için engelin nedenini belirlemeli ve engeli Spamhaus web sitesinden kaldırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="53282-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="53282-107">Kaynak IP adresinin başka birine ait olduğu engellenen gelen iletiler için adres sahibinin engeli Spamhaus web sitesinden kaldırması gerekir.</span><span class="sxs-lookup"><span data-stu-id="53282-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="53282-108">IP adresi İlke Engelleme Listesi'de (PBL) yer alıyorsa, IP adresinin sahibi farklı bir statik IP adresi atayan veya adresi PBL'den kaldırabilir.</span><span class="sxs-lookup"><span data-stu-id="53282-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="53282-109">İletiler bir üçüncü taraf hizmeti tarafından yönlendirildiyse, etki alanınıza bağlı olan engellenmiş giden iletiler için bu hatayı alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="53282-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="53282-110">Engellenmiş IP adresinin sahibini bulmak için WHOIS arama aracını kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="53282-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
