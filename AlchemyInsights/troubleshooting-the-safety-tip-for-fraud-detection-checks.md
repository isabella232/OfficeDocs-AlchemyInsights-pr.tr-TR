---
title: Dolandırıcılık algılama kontrolleri için güvenlik ipucunun giderme sorunu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759532"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="33132-102">Dolandırıcılık algılama kontrolleri için güvenlik ipucunun giderme sorunu</span><span class="sxs-lookup"><span data-stu-id="33132-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="33132-103">"Gönderen, dolandırıcılık algılama kontrollerimizi başarısız lığa uğrattı ve göründükleri kişi olmayabilir" diyen bir güvenlik ipucu alıyorsanız, gönderen DKIM veya SPF kimlik doğrulama denetimlerini geçemedi.</span><span class="sxs-lookup"><span data-stu-id="33132-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="33132-104">Bunu çözmek için en iyi yöntem, gönderenin kendilerini yetkilendirmesidir.</span><span class="sxs-lookup"><span data-stu-id="33132-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="33132-105">Gönderen sizin adınıza gönderiyorsa, gönderenin IP adresini SPF kaydınıza ekleyerek bunları yetkilendirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="33132-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="33132-106">Daha fazla bilgi [için dolandırıcılık algılama denetimleri için kırmızı (şüpheli) güvenlik ipucusorun giderme](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) bakın.</span><span class="sxs-lookup"><span data-stu-id="33132-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="33132-107">Burada yardımcı olabilecek diğer bazı bağlantılar şunlardır:</span><span class="sxs-lookup"><span data-stu-id="33132-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="33132-108">Microsoft, sızdırmayı önlemek için gönderen ilkesi çerçevesini (SPF) nasıl kullanır?</span><span class="sxs-lookup"><span data-stu-id="33132-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="33132-109">Sızdırmayı önlemeye yardımcı olmak için SPF'yi ayarlama</span><span class="sxs-lookup"><span data-stu-id="33132-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
