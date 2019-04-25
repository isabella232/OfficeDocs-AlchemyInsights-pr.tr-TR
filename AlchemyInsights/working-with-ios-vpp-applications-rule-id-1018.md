---
title: IOS VPP uygulamaları kural kimliği 1018 ile çalışma
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420504"
---
# <a name="working-with-ios-vpp-applications"></a>IOS VPP uygulamalar ile çalışma

Okuma özellikleri, kısıtlamaları ve yapmak için adımlar hakkında bilgi edinmek için [Microsoft Intune ile bir toplu satın alma programı aracılığıyla satın IOS apps yönetmek nasıl](https://docs.microsoft.com/intune/vpp-apps-ios) satın Apple toplu programı ve Microsoft Intune desteği için onu kullanın. 
  
 **Sık karşılaşılan sorunlar:** "Kullanıcılar bir IOS VPP app atadım, ancak yükleme başarısız oldu." 
  
- Birden çok mobil aygıt yönetimi sağlayıcıları tek bir VPP belirteci kullanılıyorsa, bu durum oluşabilir. Apple dan VPP belirteçleri yalnızca bir sağlayıcı ile kullanılabilir. VPP belirteci ile birden çok sağlayıcı kullandıysanız, belirtece Intune yeniden karşıya yüklemeniz gerekir.
    
- Yükleme yüklemeler sayısı toplam lisans sayısını aşarsa de başarısız olabilir. Gitmek için **Intune Mobile apps** lisanslarınızı bir kullanım raporu görüntülemek için \> **App lisans** sayfası. Kullanım lisansları geri kazanmak öğrenmek için bkz: [Bu makalede.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

