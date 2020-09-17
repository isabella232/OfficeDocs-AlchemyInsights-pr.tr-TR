---
title: SpamHaus tarafından engellenen bir e-posta gönderilirken hata oluştu
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783823"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="5b7f6-102">E-posta gönderilirken hata oluştu: Istemci ana bilgisayarı Spamhaus kullanılarak engellendi</span><span class="sxs-lookup"><span data-stu-id="5b7f6-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="5b7f6-103">İletiyi gönderen IP adresi, [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)'in sahip olduğu bir engelleme listesinde yer alıyor.</span><span class="sxs-lookup"><span data-stu-id="5b7f6-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="5b7f6-104">Spamhaus tarafından engellenmesi nedenleri, genel bir IP adresi ve Internet servis sağlayıcısı (ISS) ilkelerini paylaşan güvenliği aşılan hesaplar, güvenliği aşılan makineler içeriyor.</span><span class="sxs-lookup"><span data-stu-id="5b7f6-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="5b7f6-105">Olası düzeltmeler:</span><span class="sxs-lookup"><span data-stu-id="5b7f6-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="5b7f6-106">Kaynak e-posta sunucusunu kontrol ettiğiniz engellenen gelen iletilerde, nedeni belirlemeniz ve bloğu Spamhaus Web sitesinden kaldırmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="5b7f6-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="5b7f6-107">Kaynak IP adresinin başka birine ait olduğu engellenen gelen iletiler için, adresin sahibinin, Spamhaus Web sitesinden engellemeyi kaldırması gerekmektedir.</span><span class="sxs-lookup"><span data-stu-id="5b7f6-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="5b7f6-108">IP adresi Ilke engelleme listesinde (PBL) yer alıyorsa, sahibi farklı bir statik IP adresi atayabilir veya bu adresi PBL 'den kaldırabilir.</span><span class="sxs-lookup"><span data-stu-id="5b7f6-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="5b7f6-109">Microsoft 'a bağlı etki alanınızda engellenmiş giden iletiler için, iletiler üçüncü taraf bir hizmet üzerinden yönlendirildiyse bu hatayı alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5b7f6-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="5b7f6-110">Engellenen IP adresi sahibini bulmak için bir WHOIS arama aracı kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5b7f6-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
