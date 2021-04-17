---
title: Dolandırıcılık algılama denetimleri için güvenlik ipucu sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834751"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="58b5c-102">Dolandırıcılık algılama denetimleri için güvenlik ipucu sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="58b5c-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="58b5c-103">"Gönderen, dolandırıcılık algılama denetimlerimizi başarısız yaptı" ifadesinin yer alma olduğu bir güvenlik ipucu alıyorsanız ve bu gönderen, DKIM veya SPF kimlik doğrulama denetimlerinden geçiremedi.</span><span class="sxs-lookup"><span data-stu-id="58b5c-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="58b5c-104">Bunu çözmek için en iyi yöntem, gönderenin kendi yetkilerini vermesidir.</span><span class="sxs-lookup"><span data-stu-id="58b5c-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="58b5c-105">Gönderen sizin adınıza gönderiyorsa, gönderenin IP adresini SPF kaydınıza ekleyerek bu adrese yetki vermeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="58b5c-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="58b5c-106">Daha [fazla bilgi için bkz. Dolandırıcılık algılaması için kırmızı (şüpheli) güvenlik](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) ipucu sorunlarını giderme.</span><span class="sxs-lookup"><span data-stu-id="58b5c-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="58b5c-107">Size yardımcı olacak diğer bazı bağlantılar:</span><span class="sxs-lookup"><span data-stu-id="58b5c-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="58b5c-108">Microsoft, sender Policy Framework'i (SPF) kullanarak kimliği doğrunlamayı önlemek için nasıl kullanır?</span><span class="sxs-lookup"><span data-stu-id="58b5c-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="58b5c-109">SPF'yi, sanallık engellemeye yardımcı olacak şekilde ayarlama</span><span class="sxs-lookup"><span data-stu-id="58b5c-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
