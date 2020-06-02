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
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506866"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Uzak Masaüstü Hizmetlerinde Office 2013 etkinleştirme sırasında hata

Uzak Masaüstü Hizmetleri (RDS) dağıtımlarında Office 2013'ü etkinleştirirken bir hata alıyorsanız, kayıt defterini düzenleyerek ADAL'ı etkinleştirmeyi düşünün.
  
|**Kayıt defteri anahtarı**|**Tür**|**Değer**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Ortak\Kimlik\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Daha fazla bilgi için windows [aygıtlarında Office 2013 için Modern Kimlik Doğrulamasını Etkinleştir'e](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)bakın.
  
> [!NOTE]
>  ADAL, kurumsal ve Office 2016 için Microsoft 365 Apps'ta varsayılan olarak etkinleştirilir. Uzak Masaüstü Hizmetleri (RDS) daha önce Terminal Hizmetleri olarak adlandırıldı.
  