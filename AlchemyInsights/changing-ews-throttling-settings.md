---
title: EWS azaltma ayalarını değiştirme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075917"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="b95f1-102">EWS azaltma ayalarını değiştirme</span><span class="sxs-lookup"><span data-stu-id="b95f1-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="b95f1-103">Lütfen geçişiniz sürecince EWS azaltma ayarlarını değiştirmenize izin verecek olan otomatikleştirilmiş testi çalıştırınız. </span><span class="sxs-lookup"><span data-stu-id="b95f1-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="b95f1-104">Bu testi çalıştırmanıza rağmen, EWS içeri aktarımları yine de posta kutusu başına 5 dakikada 150 MB ile sınırlandırılacaktır; daha yüksek geçiş aktarım hızı elde etmek için lütfen daha fazla sayıdaki kullanıcının aynı anda geçiş yapmasını sağlayın. </span><span class="sxs-lookup"><span data-stu-id="b95f1-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="b95f1-105">Lütfen EWS azaltma ayarlarındaki ilke değişikliklerinin aşağıdaki (Microsoft araçları kullanan) geçiş türleri üzerinde hiç bir etkisi olmadığını unutmayınız: Karma Tam/Aşamalı (RPC/HTTP), IMAP, G Suite, Ortak Klasör ya da PST İçeri Aktarma Hizmeti.</span><span class="sxs-lookup"><span data-stu-id="b95f1-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>