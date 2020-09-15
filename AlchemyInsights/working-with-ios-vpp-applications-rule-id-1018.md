---
title: İOS VPP uygulamalarıyla çalışma kuralı 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688966"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="b8065-102">İOS VPP uygulamalarıyla çalışma</span><span class="sxs-lookup"><span data-stu-id="b8065-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="b8065-103">Apple Volume Purchase programından ve Microsoft Intune 'da sağlanan desteği kullanmanın özelliklerini, kısıtlamalarını ve adımlarını öğrenmek için, [Microsoft Intune ile bir toplu satın alma programı aracılığıyla satın alınan iOS uygulamalarını yönetmeyi](https://docs.microsoft.com/intune/vpp-apps-ios) okuyun.</span><span class="sxs-lookup"><span data-stu-id="b8065-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="b8065-104">**Sık karşılaşılan sorunlar:** "Kullanıcılarıma bir iOS VPP uygulaması atadım, ancak yükleme başarısız oldu."</span><span class="sxs-lookup"><span data-stu-id="b8065-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="b8065-105">Birden çok mobil cihaz yönetim sağlayıcısı genelinde tek bir VPP belirteci kullanılıyorsa bu olabilir.</span><span class="sxs-lookup"><span data-stu-id="b8065-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="b8065-106">Apple 'dan alınan VPP belirteçleri yalnızca bir sağlayıcı ile kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="b8065-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="b8065-107">Birden çok sağlayıcı içeren bir VPP belirteci kullandıysanız, belirteci Intune 'a yeniden yüklemelisiniz.</span><span class="sxs-lookup"><span data-stu-id="b8065-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="b8065-108">Toplam yükleme sayısı lisans sayısını aştığında de yükleme başarısız olabilir.</span><span class="sxs-lookup"><span data-stu-id="b8065-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="b8065-109">Lisanslarınız için kullanım raporunu görüntülemek için **Intune mobil uygulamalar** \> **uygulama lisansları** sayfasına gidin.</span><span class="sxs-lookup"><span data-stu-id="b8065-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="b8065-110">Lisansları kullanımda geri kazanma hakkında bilgi edinmek için [Bu makaleye bakın.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="b8065-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
