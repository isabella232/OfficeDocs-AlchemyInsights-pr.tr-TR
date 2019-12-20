---
title: Takımlar 4c7 hatası
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796440"
---
# <a name="4c7-error-in-microsoft-teams"></a>Microsoft Teams'de 4c7 hatası

Microsoft Teams Formkimlik Doğrulaması gerektirdiğinden bu hata oluşur. Active Directory Federation Services (AD FS) dağıttığınızda, Form kimlik doğrulaması varsayılan olarak intranet için etkinleştirilmez. Windows Tümleşik Kimlik Doğrulama başarısız olursa, Form kimlik doğrulaması kullanarak oturum açmanız istenir.

Bu sorunu gidermek için, Active Directory'nin yerel kopyasına sahip bilgisayarda AD FS Microsoft Yönetim Konsolu (MMC) snap-in'i kullanarak Form Kimlik Doğrulaması'nı etkinleştirin. Bunu yapmak için aşağıdaki adımları izleyin: 

1. Gezinti bölmesinde Kimlik Doğrulama **İlkeleri'ne**göz atın.
2. Ayrıntılar bölmesindeki **Eylemler** altında, **Genel Birincil Kimlik Doğrulamasını Edit'i**seçin.
3. **Intranet** sekmesinde **Form kimlik doğrulaması'nı**seçin.
4. **Tamam** 'ı (veya **Uygula'yı**) seçin.