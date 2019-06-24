---
title: OneDrive içinde 0x8004de40 hata düzeltme
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133996"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>OneDrive içinde 0x8004de40 hata düzeltme

OneDrive ile 0x8004de40 hata alırsanız:

- Acitve Directory etki alanına bağlıyken etkilenen bilgisayarı yeniden başlatın.
- Yeniden başlatma sorunu gidermezse, ayrılma ve aygıtınızdan Azure AD alanına yeniden katın. 

**Not**: aşağıdaki adımları gerçekleştirirken, şirket ağınızda olmalısınız. (Örneğin, seyahat ederken) şirket altyapınızı bağlanmak mümkün değildir, bu adımları gerçekleştirmeyin. 

- Yükseltilmiş bir komut istemi açın. 
- Yükseltilmiş bir komut istemi açmak için **Başlat**' ı tıklatın -, **komut istemini**sağ tıklatın ve sonra **yönetici olarak çalıştır**' ı tıklatın.
- *Dsregcmd /leave* yazın ve **Enter**tuşuna basın.
- Tamamlandığında, *dsregcmd /join* yazın ve **Enter**tuşuna basın.
- Tamamlandığında komut istemini kapatın.
- Bilgisayarı yeniden başlatıp oturum OneDrive.