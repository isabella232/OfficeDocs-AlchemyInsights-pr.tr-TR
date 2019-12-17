---
title: OneDrive'da 0x8004de40 hatasini düzeltin
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052057"
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