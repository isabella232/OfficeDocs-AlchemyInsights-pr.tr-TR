---
title: iOS VPP Uygulamaları ile Çalışma Kural Id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719977"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="bcccd-102">iOS VPP Uygulamaları ile Çalışma</span><span class="sxs-lookup"><span data-stu-id="bcccd-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="bcccd-103">Apple Toplu Satın Alma Programı'ndan ve Microsoft Intune'da bu programa yönelik destekten yararlanmak için microsoft [Intune ile toplu satın alma programı aracılığıyla satın alınan iOS uygulamalarını nasıl](https://docs.microsoft.com/intune/vpp-apps-ios) yönetebilirsiniz'i okuyun.</span><span class="sxs-lookup"><span data-stu-id="bcccd-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="bcccd-104">**Sık Karşılaşılan Sorunlar:** "Kullanıcılarıma bir iOS VPP uygulaması atadim, ancak yükleme başarısız oldu."</span><span class="sxs-lookup"><span data-stu-id="bcccd-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="bcccd-105">Tek bir VPP belirteci birden çok mobil cihaz yönetim sağlayıcısında kullanılırsa bu durum olabilir.</span><span class="sxs-lookup"><span data-stu-id="bcccd-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="bcccd-106">Apple'ın VPP belirteçleri yalnızca tek bir sağlayıcıda kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="bcccd-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="bcccd-107">Birden çok sağlayıcıiçeren bir VPP belirteci kullandıysanız, belirteci Intune'a yeniden yüklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="bcccd-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="bcccd-108">Toplam yükleme sayısı lisans sayısını aşarsa yükleme de başarısız olabilir.</span><span class="sxs-lookup"><span data-stu-id="bcccd-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="bcccd-109">Lisanslarınız için kullanım raporunu görüntülemek için **Intune Mobile uygulamaları** \> **Uygulaması lisansları** sayfasına gidin.</span><span class="sxs-lookup"><span data-stu-id="bcccd-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="bcccd-110">Kullanılan lisansları nasıl geri alacağız'u öğrenmek için [bu makaleye bakın.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="bcccd-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
