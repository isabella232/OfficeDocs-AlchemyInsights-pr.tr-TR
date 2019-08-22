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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525079"
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