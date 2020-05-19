---
title: Bir etki alanını veya e-posta göndereni güvenli olarak işaretlemeli mi?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281239"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="35ee3-102">Bir etki alanını veya e-posta göndereni güvenli olarak işaretlemeli mi?</span><span class="sxs-lookup"><span data-stu-id="35ee3-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="35ee3-103">Güvenli gönderen listelerinin kullanılması, kuruluşunuzun spam, kimlik avı ve sahte ciponasyon saldırılarına açık olması **için önerilmez.**</span><span class="sxs-lookup"><span data-stu-id="35ee3-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="35ee3-104">Ancak, bir iş gereksinimi varsa, bunun için Posta Akışı **Kuralları'nı kullanmanızı öneririz.** **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**</span><span class="sxs-lookup"><span data-stu-id="35ee3-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="35ee3-105">Kılavuzumuz gönderenin kimlik doğrulamasını sağlar (alan adı göndermenin sahte olmadığını doğrular).</span><span class="sxs-lookup"><span data-stu-id="35ee3-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="35ee3-106">**Not**: Spam filtrelemenin istisnaları kuruluşunuzu güvenlik saldırılarına açabileceğinden, güvenli gönderen listeleri kullanarak yanlış pozitif leri yönetmenizi önermiyoruz.</span><span class="sxs-lookup"><span data-stu-id="35ee3-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="35ee3-107">Kullanıcınız spam veya önemsiz e-posta olarak yanlış işaretlenmiş iletiler alıyorsa, lütfen **[iletileri ve dosyaları Microsoft'a bildirin.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="35ee3-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="35ee3-108">Gönderenler tüm spam, sahtekarlık ve kimlik avı korumasını ve gönderen kimlik doğrulamasını (SPF, DKIM, DMARC) atladığı için, Outlook'taki Güvenli Gönderenler, İzin Verilen gönderenler listesinden veya istenmeyen posta önleme politikalarında izin verilen etki alanı listesinden **kaçınılmalıdır.**</span><span class="sxs-lookup"><span data-stu-id="35ee3-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="35ee3-109">Bu yöntem en iyi yalnızca geçici sınama için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="35ee3-109">This method is best used for temporary testing only.</span></span>
