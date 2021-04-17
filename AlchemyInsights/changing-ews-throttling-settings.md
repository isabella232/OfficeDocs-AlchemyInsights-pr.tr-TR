---
title: EWS azaltma ayarlarını değiştirme
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818056"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="b3875-102">EWS azaltma ayarlarını değiştirme</span><span class="sxs-lookup"><span data-stu-id="b3875-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="b3875-103">Lütfen geçişiniz süresince EWS azaltma ilkesini değiştirmenize olanak verecek olan otomatikleştirilmiş testi çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="b3875-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="b3875-104">Bu testi çalıştırmanıza rağmen, EWS içeri aktarımları yine de posta kutusu başına 5 dakikada 150 MB ile sınırlandırılacaktır; daha yüksek geçiş aktarım hızı elde etmek için lütfen daha fazla sayıdaki kullanıcının aynı anda geçiş yapmasını sağlayın.</span><span class="sxs-lookup"><span data-stu-id="b3875-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="b3875-105">Lütfen EWS azaltma ilkesi değişikliklerinin aşağıdaki Microsoft araçlarını kullanan geçiş türleri üzerinde hiçbir etkisi olmadığını unutmayın: Karma Tam/Aşamalı (RPC/HTTP), IMAP, G Suite, Ortak Klasör ya da PST İçeri Aktarma Hizmeti.</span><span class="sxs-lookup"><span data-stu-id="b3875-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>