---
title: Etki alanı veya e-posta gönderenini güvenli olarak işaretlemelisiniz mi gerekiyor?
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
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803265"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="44ed9-102">Etki alanı veya e-posta gönderenini güvenli olarak işaretlemelisiniz mi gerekiyor?</span><span class="sxs-lookup"><span data-stu-id="44ed9-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="44ed9-103">Kuruluşunuzu istenmeyen posta, sızdırma ve sızdırma saldırılarına karşı açtığından **güvenli gönderen listelerinin kullanımı önerilmez** .</span><span class="sxs-lookup"><span data-stu-id="44ed9-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="44ed9-104">Bununla birlikte, iş gereksinimi varsa, bunun için **[posta akış kurallarını](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** kullanmanızı **öneririz** .</span><span class="sxs-lookup"><span data-stu-id="44ed9-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="44ed9-105">Kılavuzumuz, Gönderen kimlik doğrulamasını garantiler (etki alanı göndermeyi doğrular.).</span><span class="sxs-lookup"><span data-stu-id="44ed9-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="44ed9-106">**Not**: istenmeyen filtreleme özel durumları kuruluşunuzun güvenlik saldırılarına karşı açabildiğinden, güvenli gönderen listelerini kullanarak yanlış pozitif durumları yönetmeniz önerilmez.</span><span class="sxs-lookup"><span data-stu-id="44ed9-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="44ed9-107">Kullanıcılarınız iletileri yanlışlıkla istenmeyen posta veya gereksiz e-posta olarak alıyorsa, lütfen **[iletileri ve dosyaları Microsoft 'A bildirin](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="44ed9-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="44ed9-108">Gönderenler, istenmeyen posta önleme, sızma ve bir istenmeyen postayı devre dışı bırakabilir ve Gönderen kimlik **should be avoided** doğrulaması (SPF, CıKIM, DMARC) gibi</span><span class="sxs-lookup"><span data-stu-id="44ed9-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="44ed9-109">Bu yöntem yalnızca geçici test için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="44ed9-109">This method is best used for temporary testing only.</span></span>
