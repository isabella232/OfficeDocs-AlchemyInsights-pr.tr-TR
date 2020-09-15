---
title: Sahtekarlık algılaması denetimlerinde güvenlik ipucu sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658430"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="c39d1-102">Sahtekarlık algılaması denetimlerinde güvenlik ipucu sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="c39d1-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="c39d1-103">"Gönderen sahtekarlık algılaması denetimlerinde başarısız oldu ve" gönderdikleri kişiler olmayabilir "ifadesini içeren bir güvenlik ipucu alıyorsanız, gönderen tüm vaya veya SPF kimlik doğrulama denetimlerini geçemedi.</span><span class="sxs-lookup"><span data-stu-id="c39d1-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="c39d1-104">Bunu çözmenin en iyi yöntemi, gönderenin kendilerine yetki vermek içindir.</span><span class="sxs-lookup"><span data-stu-id="c39d1-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="c39d1-105">Gönderen sizin adınıza gönderiyorsanız, gönderenin IP adresini SPF kaydınıza ekleyerek onlara yetki vermeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="c39d1-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="c39d1-106">Daha fazla bilgi için, [sahte algılama denetimlerinde kırmızı (şüpheli) güvenlik Ipucunda sorun giderme](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="c39d1-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="c39d1-107">İşte size yardımcı olabilecek diğer bağlantılar:</span><span class="sxs-lookup"><span data-stu-id="c39d1-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="c39d1-108">Microsoft 'un, sahtekarlık ilkesini</span><span class="sxs-lookup"><span data-stu-id="c39d1-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="c39d1-109">Yanıltlığa engel olma</span><span class="sxs-lookup"><span data-stu-id="c39d1-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
