---
title: OneDrive'da 0x8004de40 hatasini düzeltin
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716048"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>OneDrive'da 0x8004de40 hatasini düzeltin

OneDrive ile 0x8004de40 hatası alırsanız:

- Acitve Directory etki alanınıza bağlıyken etkilenen bilgisayarı yeniden başlatın.
- Yeniden başlatma sorunu çözmezse, Azure AD'den cihazınıza katılın ve yeniden katılın. 

**Not**: Bu adımları gerçekleştirirken şirket ağınızda olmalısınız. Kurumsal altyapınıza bağlanamadığınızda (örneğin, seyahat ederken) bu adımları gerçekleştirin. 

- Yükseltilmiş bir komut istemini açın. 
- Yükseltilmiş komut istemini açmak için - **Başlat,** **Komut İstem'i**sağ tıklatın ve ardından **yönetici olarak çalıştır'ı**tıklatın.
- *Dsregcmd* yazın /bırak ve **Enter**tuşuna basın.
- Tamamlandığında, *dsregcmd yazın /join* ve **Enter**tuşuna basın.
- Tamamlandığında, komut istemini kapatın.
- Bilgisayarı yeniden başlatın ve OneDrive'a giriş yapın.