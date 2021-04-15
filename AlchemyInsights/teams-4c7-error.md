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
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786689"
---
# <a name="4c7-error-in-microsoft-teams"></a>Microsoft Teams'de 4c7 hatası

Bu hata, Microsoft Teams'de Forms Authentication'ın gerekli olduğu için oluşur. Active Directory Federasyon Hizmetleri'nin (AD FS) dağıtımında, Forms Kimlik Doğrulaması intranet için varsayılan olarak etkinleştirilmez. Windows Tümleşik Kimlik Doğrulaması başarısız olursa, Forms Authentication'ı kullanarak oturum açmanız istenir.

Bu sorunu çözmek için, Active Directory'nin yerel kopyasına sahip bilgisayarda AD FS Microsoft Yönetim Konsolu (MMC) ek bileşenini kullanarak Forms Kimlik Doğrulamasını etkinleştirin. Bunu yapmak için şu adımları uygulayın: 

1. Gezinti bölmesinde Kimlik Doğrulama İlkeleri'ne **gidin.**
2. Ayrıntılar **bölmesindeki** Eylemler'in altında Genel Birincil Kimlik **Doğrulamayı Düzenle'yi seçin.**
3. Intranet sekmesinde **Forms** Authentication öğesini **seçin.**
4. **Tamam'ı** (veya **Uygula'yi) seçin.**