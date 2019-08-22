---
title: SpamHaus tarafından engellenen e-posta gönderme hatası
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 39213f6f1b96c2bef9ea071f43c38766debf64d1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527162"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="78617-102">E-posta gönderilirken hata: istemci ana bilgisayar Spamhaus kullanılarak engellendi</span><span class="sxs-lookup"><span data-stu-id="78617-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="78617-103">[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)tarafından sahip olunan bir engelleme listesindeki iletiyi gönderen IP adresi var.</span><span class="sxs-lookup"><span data-stu-id="78617-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="78617-104">Spamhaus tarafından engellenmesini için nedenleri ele geçirilen hesapları, ortak bir IP adresi ve Internet servis sağlayıcısı (ISS) ilkelerini paylaşma makineleri tehlikeye.</span><span class="sxs-lookup"><span data-stu-id="78617-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="78617-105">Olası düzeltmeler şunlardır:</span><span class="sxs-lookup"><span data-stu-id="78617-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="78617-106">Office kaynak e-posta sunucusu kontrol burada 365 engellenen gelen iletiler için nedenini belirlemek ve blok Spamhaus Web sitesinden kaldırmak gerekir.</span><span class="sxs-lookup"><span data-stu-id="78617-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="78617-107">Kaynak IP adresini başka bir kişiye ait olduğu Office 365 engellenen gelen iletiler için adres sahibi blok Spamhaus Web sitesinden kaldırmak gerekir.</span><span class="sxs-lookup"><span data-stu-id="78617-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="78617-108">IP adresi İlkesi engelleme listesi (PBL) ise, sahibi PBL adresi kaldırın veya farklı bir statik IP adresi atayın.</span><span class="sxs-lookup"><span data-stu-id="78617-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="78617-109">Office 365 etki alanınızdan engellenen giden iletiler için bu hata iletileri bir 3 parti hizmeti üzerinden yönlendirilir alabilir.</span><span class="sxs-lookup"><span data-stu-id="78617-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="78617-110">Engellenen IP adresi sahibi bulmak için bir WHOIS arama aracını kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="78617-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
