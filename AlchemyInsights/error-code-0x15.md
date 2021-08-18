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
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316706"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Uzak Masaüstü Hizmetleri'Office 2013 etkinleştirme hatası

Uzak Masaüstü Hizmetleri (RDS) dağıtımlarında Office 2013'ü etkinleştirirken hata alıyorsanız, ADAL'yi kayıt defterini düzenleyerek etkinleştirmeyi göz önünde bulundurabilirsiniz.
  
|**Kayıt defteri anahtarı**|**Tür**|**Değer**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Daha fazla bilgi için [bkz. Office 2013](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)için Modern Kimlik Doğrulamayı Windows.
  
**Not:** Kurumlar için Microsoft 365 Uygulamaları ve Office 2016'da ADAL varsayılan olarak etkindir. Uzak Masaüstü Hizmetleri (RDS) daha önce Terminal Hizmetleri olarak adlandırılmıştır.
  