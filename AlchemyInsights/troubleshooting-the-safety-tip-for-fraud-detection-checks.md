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
ms.openlocfilehash: 98627edcd2b685673dda8a8a18821eddf9b64bc1
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391229"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="3e047-102">Sahtekarlık algılama için emniyet ipucu sorun giderme denetler</span><span class="sxs-lookup"><span data-stu-id="3e047-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="3e047-103">Siz iseniz, emniyet ipucu alma "gönderen bizim sahtekarlık algılama denetimlerinde başarısız oldu ve kim gibi görünüyor olabilir" diyor, sonra gönderen DKIM veya SPF kimlik doğrulama denetimleri geçmek başarısız oldu.</span><span class="sxs-lookup"><span data-stu-id="3e047-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="3e047-104">Gönderen kendilerini yetkilendirmek bu sorunu çözmek için en iyi yöntemdir.</span><span class="sxs-lookup"><span data-stu-id="3e047-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="3e047-105">Gönderen sizin adınıza gönderilmesi, Gönderenin IP adresi SPF kaydınızı ekleyerek yetkilendirmek gerekir.</span><span class="sxs-lookup"><span data-stu-id="3e047-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="3e047-106">[Sahtekarlık algılama için kırmızı (şüpheli) emniyet ipucu sorun giderme denetler](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) , daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="3e047-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="3e047-107">Yardımcı olabilecek diğer bazı bağlantılar şunlardır:</span><span class="sxs-lookup"><span data-stu-id="3e047-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="3e047-108">Gönderen ilke çerçevesi (SPF) Office 365 sahtekarlığı önlemek için nasıl kullanır</span><span class="sxs-lookup"><span data-stu-id="3e047-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="3e047-109">Kimlik sahtekarlığını önlemeye yardımcı olmak için Office 365'te SPF'yi ayarlama</span><span class="sxs-lookup"><span data-stu-id="3e047-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

