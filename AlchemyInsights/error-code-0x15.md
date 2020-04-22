---
title: Hata Kodu 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Uzak Masaüstü Hizmetleri (RDS) dağıtımlarında Office 2013'ü etkinleştirirken bir hata alıyorsanız, kayıt defterini düzenleyerek ADAL'ı etkinleştirmeyi düşünün.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703158"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Uzak Masaüstü Hizmetlerinde Office 2013 etkinleştirme sırasında hata

Uzak Masaüstü Hizmetleri (RDS) dağıtımlarında Office 2013'ü etkinleştirirken bir hata alıyorsanız, kayıt defterini düzenleyerek ADAL'ı etkinleştirmeyi düşünün.
  
|**Kayıt defteri anahtarı**|**Tür**|**Değer**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Ortak\Kimlik\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

Daha fazla bilgi için windows [aygıtlarında Office 2013 için Modern Kimlik Doğrulamasını Etkinleştir'e](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)bakın.
  
> [!NOTE]
>  ADAL, kurumsal ve Office 2016 için Microsoft 365 Apps'ta varsayılan olarak etkinleştirilir. Uzak Masaüstü Hizmetleri (RDS) daha önce Terminal Hizmetleri olarak adlandırıldı.
  