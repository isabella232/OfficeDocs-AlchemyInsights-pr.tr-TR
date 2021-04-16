---
title: Etki alanını veya e-posta göndereni güvenli olarak işaretlemeniz mi gerekiyor?
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
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792152"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="d340e-102">Etki alanını veya e-posta göndereni güvenli olarak işaretlemeniz mi gerekiyor?</span><span class="sxs-lookup"><span data-stu-id="d340e-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="d340e-103">Güvenli gönderen **listelerinin kullanılması önerilmez,** çünkü kuruluş istenmeyen posta, kimlik avı ve kimlik avı saldırılarına karşı açılır.</span><span class="sxs-lookup"><span data-stu-id="d340e-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="d340e-104">Bununla birlikte, bir iş gereksinimi varsa, **bunun için Posta** **[Akış Kuralları'nın kullanılması](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** önerilir.</span><span class="sxs-lookup"><span data-stu-id="d340e-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="d340e-105">Kılavuzlarımız gönderen kimlik doğrulamasını (etki alanı göndermenin kimlik doğrulamasının kimlik doğrulaması olmadığını doğrular) sağlar.</span><span class="sxs-lookup"><span data-stu-id="d340e-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="d340e-106">**Not:** İstenmeyen posta filtreleme özel durumları güvenlik saldırılarına karşı kurumlarınızı aç etkileyecer, bunun için güvenilir gönderen listeleri kullanarak hatalı pozitif sonuç yönetimine izin veririz.</span><span class="sxs-lookup"><span data-stu-id="d340e-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="d340e-107">Kullanıcınız yanlışlıkla istenmeyen veya gereksiz e-posta olarak işaretlenmiş iletileri alırsa, lütfen İletileri ve **[dosyaları Microsoft'a rapor edin.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="d340e-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="d340e-108">Outlook'ta Güvenilir Gönderenler, İzin verilen gönderenler listesi  veya istenmeyen posta önleme ilkelerde izin verilen etki alanı listesi, gönderenler tüm istenmeyen postayı, kimlik avını ve kimlik avını (SPF, DKIM, DMARC) atlayamalarından kaçınılmalıdır.</span><span class="sxs-lookup"><span data-stu-id="d340e-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="d340e-109">Bu yöntem, yalnızca geçici test için en iyi yöntemdir.</span><span class="sxs-lookup"><span data-stu-id="d340e-109">This method is best used for temporary testing only.</span></span>
