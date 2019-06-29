---
title: Sahtekarlık algılama için emniyet ipucu sorun giderme denetler
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: ab7bd3ec66640d66e5f1ea7c1eeee0a1a9510241
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353269"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="03f1f-102">Sahtekarlık algılama için emniyet ipucu sorun giderme denetler</span><span class="sxs-lookup"><span data-stu-id="03f1f-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="03f1f-103">Siz iseniz, emniyet ipucu alma "gönderen bizim sahtekarlık algılama denetimlerinde başarısız oldu ve kim gibi görünüyor olabilir" diyor, sonra gönderen DKIM veya SPF kimlik doğrulama denetimleri geçmek başarısız oldu.</span><span class="sxs-lookup"><span data-stu-id="03f1f-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="03f1f-104">Gönderen kendilerini yetkilendirmek bu sorunu çözmek için en iyi yöntemdir.</span><span class="sxs-lookup"><span data-stu-id="03f1f-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="03f1f-105">Gönderen sizin adınıza gönderilmesi, Gönderenin IP adresi SPF kaydınızı ekleyerek yetkilendirmek gerekir.</span><span class="sxs-lookup"><span data-stu-id="03f1f-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="03f1f-106">[Sahtekarlık algılama için kırmızı (şüpheli) emniyet ipucu sorun giderme denetler](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) , daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="03f1f-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="03f1f-107">Yardımcı olabilecek diğer bazı bağlantılar şunlardır:</span><span class="sxs-lookup"><span data-stu-id="03f1f-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="03f1f-108">Gönderen ilke çerçevesi (SPF) Office 365 sahtekarlığı önlemek için nasıl kullanır</span><span class="sxs-lookup"><span data-stu-id="03f1f-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="03f1f-109">Kimlik sahtekarlığını önlemeye yardımcı olmak için Office 365'te SPF'yi ayarlama</span><span class="sxs-lookup"><span data-stu-id="03f1f-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
