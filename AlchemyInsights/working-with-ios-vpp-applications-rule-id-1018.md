---
title: IOS VPP uygulamaları kural kimliği 1018 ile çalışma
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29494803"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="31aab-102">IOS VPP uygulamalar ile çalışma</span><span class="sxs-lookup"><span data-stu-id="31aab-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="31aab-103">Okuma özellikleri, kısıtlamaları ve yapmak için adımlar hakkında bilgi edinmek için [Microsoft Intune ile bir toplu satın alma programı aracılığıyla satın IOS apps yönetmek nasıl](https://docs.microsoft.com/intune/vpp-apps-ios) satın Apple toplu programı ve Microsoft Intune desteği için onu kullanın.</span><span class="sxs-lookup"><span data-stu-id="31aab-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="31aab-104">**Sık karşılaşılan sorunlar:** "Kullanıcılar bir IOS VPP app atadım, ancak yükleme başarısız oldu."</span><span class="sxs-lookup"><span data-stu-id="31aab-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="31aab-p101">Birden çok mobil aygıt yönetimi sağlayıcıları tek bir VPP belirteci kullanılıyorsa, bu durum oluşabilir. Apple dan VPP belirteçleri yalnızca bir sağlayıcı ile kullanılabilir. VPP belirteci ile birden çok sağlayıcı kullandıysanız, belirtece Intune yeniden karşıya yüklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="31aab-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="31aab-p102">Yükleme yüklemeler sayısı toplam lisans sayısını aşarsa de başarısız olabilir. Gitmek için **Intune Mobile apps** lisanslarınızı bir kullanım raporu görüntülemek için \> **App lisans** sayfası. Kullanım lisansları geri kazanmak öğrenmek için bkz: [Bu makalede.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="31aab-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

