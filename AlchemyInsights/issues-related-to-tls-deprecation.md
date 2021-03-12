---
title: TLS 1.0 ve TLS 1.1 devre dışı bırakılama nedeniyle Office 365'e e-posta gönderemiyor/alınamıyor
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747113"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="df616-102">TLS 1.0 ve TLS 1.1 devre dışı bırakılama nedeniyle Office 365'e e-posta gönderemiyor/alınamıyor</span><span class="sxs-lookup"><span data-stu-id="df616-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="df616-103">MC229914 sonrası ileti merkezi tarafından onaylandırıldı ve TLS 1.0 ve TLS 1.1 kullanımdan çıktı.</span><span class="sxs-lookup"><span data-stu-id="df616-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="df616-104">Yakında Office 365 dış kaynaklardan TLS 1.0 ve TLS 1.1 e-posta bağlantılarını kabul etmiyor.</span><span class="sxs-lookup"><span data-stu-id="df616-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="df616-105">Ayrıca, Exchange Online giden e-posta göndermek için hiçbir zaman TLS 1.0 veya 1.1 kullanmaz.</span><span class="sxs-lookup"><span data-stu-id="df616-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="df616-106">TLS 1.0 veya 1.1 devre dışı bırakıı nedeniyle sorunlar ile karşı karşıyaysanız, aşağıdaki hatalardan birini kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="df616-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="df616-107">Gönderen NDR geri geri dönüyor - '421 4.4.2 Yuva Hatana Bağlı Bağlantı bırakıldı'</span><span class="sxs-lookup"><span data-stu-id="df616-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="df616-108">'421 4.4.2 SocketError' nedeniyle e-posta gönderen Şirket İçi Sunucusunun Sıra Görüntüleyicisi'nde hata oluştu</span><span class="sxs-lookup"><span data-stu-id="df616-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="df616-109">Office 365'e e-posta gönderen sunucuda Bağlayıcı Protokolü Gönder günlüğünde hata oluştu- TLS görüşmeleri YuvaKor hatasıyla başarısız oldu [](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging)</span><span class="sxs-lookup"><span data-stu-id="df616-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="df616-110">Bağlayıcı protokolü gönderme veya alma günlüğünde hata - '451 5.7.3 Önce STARTTLS komutu olmalı'</span><span class="sxs-lookup"><span data-stu-id="df616-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="df616-111">Yukarıdaki hatalardan herhangi birini görüyorsanız, lütfen e-posta gönderen veya alan sunucunun AŞAĞıDAKI kayıt defteri anahtarlarını kontrol ederek TLS 1.2'nin etkinleştirildiğinden emin olun:</span><span class="sxs-lookup"><span data-stu-id="df616-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="df616-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\İstemci] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span><span class="sxs-lookup"><span data-stu-id="df616-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="df616-113">Yukarıdaki kayıt defteri anahtarlarında TLS 1.2'yi etkinleştirmek için herhangi bir değişiklik yaptısanız, değişikliklerin etkin olması için sunucuyu yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="df616-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="df616-114">Ayrıca, en son Windows ve Exchange güncelleştirmelerinin yüklü olduğundan da emin olun.</span><span class="sxs-lookup"><span data-stu-id="df616-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="df616-115">Daha fazla bilgi için bkz.:</span><span class="sxs-lookup"><span data-stu-id="df616-115">For more information, see:</span></span>

- [<span data-ttu-id="df616-116">Exchange Server TLS kılavuzu, bölüm 1: TLS 1.2 için Hazırlanıyor - Microsoft Tech Topluluğu</span><span class="sxs-lookup"><span data-stu-id="df616-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="df616-117">Exchange Server TLS kılavuzu Bölüm 2: TLS 1.2'yi etkinleştirme ve Kullan kullanmayan istemcileri tanımlama - Microsoft Tech Topluluğu</span><span class="sxs-lookup"><span data-stu-id="df616-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="df616-118">TLS sürümleri Exchange Online ile kabul edilemezse e-posta senaryolarını anlama - Microsoft Tech Topluluğu</span><span class="sxs-lookup"><span data-stu-id="df616-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
