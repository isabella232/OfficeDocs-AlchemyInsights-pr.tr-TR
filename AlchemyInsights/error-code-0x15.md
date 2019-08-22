---
title: Hata kodu 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Uzak Masaüstü Hizmetleri (RDS) dağıtımları üzerinde Office 2013 etkinleştirilirken bir hata almak, kayıt defterini düzenleyerek ADAL etkinleştirme düşünün.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527087"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Uzak Masaüstü Hizmetleri üzerine Office 2013 etkinleştirme hatası

Uzak Masaüstü Hizmetleri (RDS) dağıtımları üzerinde Office 2013 etkinleştirilirken bir hata almak, kayıt defterini düzenleyerek ADAL etkinleştirme düşünün.
  
|**Kayıt defteri anahtarı**|**Tür**|**Değer**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Daha fazla bilgi için bkz: [Etkinleştirmek Modern kimlik doğrulaması Windows cihazlarda Office 2013](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL Office 365 ProPlus ve Office 2016 varsayılan olarak etkindir. Uzak Masaüstü Hizmetleri (RDS), önceden Terminal Hizmetleri olarak biliniyordu.
  