---
title: Hata kodu 0x15
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
description: Uzak Masaüstü Hizmetleri (RDS) dağıtımlarında Office 2013 ' i etkinleştirirken hata alıyorsanız, kayıt defterini düzenleyerek ADAL 'i etkinleştirmeyi düşünebilirsiniz.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709207"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Uzak Masaüstü Hizmetleri 'nde Office 2013 etkinleştirme hatası

Uzak Masaüstü Hizmetleri (RDS) dağıtımlarında Office 2013 ' i etkinleştirirken hata alıyorsanız, kayıt defterini düzenleyerek ADAL 'i etkinleştirmeyi düşünebilirsiniz.
  
|**Kayıt defteri anahtarı**|**Tür**|**Değer**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |2  <br/> |

Daha fazla bilgi için [Windows cihazlarında Office 2013 Için modern kimlik doğrulamasını etkinleştirme](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)konusuna bakın.
  
> [!NOTE]
>  ADAL, kurumsal ve Office 2016 için Microsoft 365 uygulamalarında varsayılan olarak etkinleştirilmiştir. Uzak Masaüstü Hizmetleri (RDS) daha önce Terminal Hizmetleri olarak adlandırıyordu.
  