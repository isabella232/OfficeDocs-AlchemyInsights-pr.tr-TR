---
title: Hata kodu 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Uzak Masaüstü Hizmetleri (RDS) dağıtımları üzerinde Office 2013 etkinleştirilirken bir hata almak, kayıt defterini düzenleyerek ADAL etkinleştirme düşünün.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402759"
---
Uzak Masaüstü Hizmetleri (RDS) dağıtımları üzerinde Office 2013 etkinleştirilirken bir hata almak, kayıt defterini düzenleyerek ADAL etkinleştirme düşünün. 
  
|**Kayıt defteri anahtarı**|**Tür**|**Değer**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Daha fazla bilgi için bkz: [Etkinleştirmek Modern kimlik doğrulaması Windows cihazlarda Office 2013](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL Office 365 ProPlus ve Office 2016 varsayılan olarak etkindir. > Uzak Masaüstü Hizmetleri (RDS), önceden Terminal Hizmetleri olarak biliniyordu. 
  

