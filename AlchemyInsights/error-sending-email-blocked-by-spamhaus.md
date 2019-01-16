---
title: SpamHaus tarafından engellenen e-posta gönderme hatası
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28318185"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="c0d9a-102">E-posta gönderilirken hata: istemci ana bilgisayar Spamhaus kullanılarak engellendi</span><span class="sxs-lookup"><span data-stu-id="c0d9a-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="c0d9a-p101">[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)tarafından sahip olunan bir engelleme listesindeki iletiyi gönderen IP adresi var. Spamhaus tarafından engellenmesini için nedenleri ele geçirilen hesapları, ortak bir IP adresi ve Internet servis sağlayıcısı (ISS) ilkelerini paylaşma makineleri tehlikeye. Olası düzeltmeler şunlardır:</span><span class="sxs-lookup"><span data-stu-id="c0d9a-p101">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies. Possible fixes are:</span></span>
  
- <span data-ttu-id="c0d9a-106">Office kaynak e-posta sunucusu kontrol burada 365 engellenen gelen iletiler için nedenini belirlemek ve blok Spamhaus Web sitesinden kaldırmak gerekir.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="c0d9a-p102">Kaynak IP adresini başka bir kişiye ait olduğu Office 365 engellenen gelen iletiler için adres sahibi blok Spamhaus Web sitesinden kaldırmak gerekir. IP adresi İlkesi engelleme listesi (PBL) ise, sahibi PBL adresi kaldırın veya farklı bir statik IP adresi atayın.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-p102">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website. If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="c0d9a-p103">Office 365 etki alanınızdan engellenen giden iletiler için bu hata iletileri bir 3 parti hizmeti üzerinden yönlendirilir alabilir. Engellenen IP adresi sahibi bulmak için bir WHOIS arama aracını kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-p103">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service. You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

