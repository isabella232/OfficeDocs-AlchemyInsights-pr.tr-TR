---
title: Teams 4c7 hatası
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049328"
---
# <a name="4c7-error-in-microsoft-teams"></a>Microsoft Teams'ta 4c7 Microsoft Teams

Bu hata, kimlik doğrulamasının Forms Microsoft Teams gerektirdiği için oluşur. Active Directory Federasyon Hizmetleri'nin (AD FS) dağıtımında, Forms Kimlik Doğrulaması intranet için varsayılan olarak etkinleştirilmez. Tümleşik Windows başarısız olursa, Forms Authentication'ı kullanarak oturum açmanız istenir.

Bu sorunu çözmek için, Active Directory'nin yerel kopyasına sahip bilgisayarda AD FS Microsoft Yönetim Konsolu (MMC) ek bileşenini kullanarak Forms Kimlik Doğrulamasını etkinleştirin. Bunu yapmak için şu adımları uygulayın: 

1. Gezinti bölmesinde Kimlik Doğrulama İlkeleri'ne **gidin.**
2. Ayrıntılar **bölmesindeki** Eylemler'in altında Genel Birincil Kimlik **Doğrulamayı Düzenle'yi seçin.**
3. Intranet sekmesinde **Forms** Authentication öğesini **seçin.**
4. **Tamam'ı** (veya **Uygula'yi) seçin.**