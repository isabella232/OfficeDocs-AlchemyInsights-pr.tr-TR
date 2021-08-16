---
title: Hata Kodu 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Uzak Masaüstü Hizmetleri (RDS) dağıtımlarında Office 2013'ü etkinleştirirken hata alıyorsanız, ADAL'yi kayıt defterini düzenleyerek etkinleştirmeyi göz önünde bulundurabilirsiniz.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100782"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Uzak Masaüstü Hizmetleri'Office 2013 etkinleştirme hatası

Uzak Masaüstü Hizmetleri (RDS) dağıtımlarında Office 2013'ü etkinleştirirken hata alıyorsanız, ADAL'yi kayıt defterini düzenleyerek etkinleştirmeyi göz önünde bulundurabilirsiniz.
  
|**Kayıt defteri anahtarı**|**Tür**|**Değer**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Daha fazla bilgi için [bkz. Mobil cihazlarda Office 2013](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)için Modern kimlik Windows etkinleştirme .
  
> [!NOTE]
>  Kurumlar için Microsoft 365 Uygulamaları 2016'da ADAL Office etkindir. Uzak Masaüstü Hizmetleri (RDS) daha önce Terminal Hizmetleri olarak adlandırılmıştır.
  