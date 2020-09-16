---
title: OneDrive 'da 0x8004de40 hatasını düzeltme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745150"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>OneDrive 'da 0x8004de40 hatasını düzeltme

OneDrive ile bir 0x8004de40 hatası alıyorsanız:

- Acitve dizin etki alanınıza bağlıyken etkilenen bilgisayarı yeniden başlatın.
- Yeniden yükleme sorunu çözmezse, aboneliğinizi kaldırın ve cihazınızı Azure AD 'den yeniden katın. 

**Not**: Bu adımları uygularken şirket ağınızda olmalısınız. Şirket altyapısına (örneğin, seyahat halindeyken) bağlanamadığınızda bu adımları kullanmayın. 

- Yükseltilmiş bir komut istemi açın. 
- Yükseltilmiş bir komut istemini açmak için- **Başlat**'a tıklayın, **komut istemi**'ne sağ tıklayın ve **yönetici olarak Run**'a tıklayın.
- *Dsregcmd/Leave* yazın ve **ENTER**tuşuna basın.
- Tamamlandığında *dsregcmd/Join* yazın ve **ENTER**tuşuna basın.
- Tamamlandığında komut istemini kapatın.
- Bilgisayarı yeniden başlatın ve OneDrive 'da oturum açın.