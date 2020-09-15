---
title: Ekipler 4c7 hatası
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700223"
---
# <a name="4c7-error-in-microsoft-teams"></a>Microsoft ekiplerde 4c7 hatası

Bu hata, Microsoft ekipleri Forms kimlik doğrulaması gerektirdiğinden oluşur. Active Directory Federasyon Hizmetleri 'ni (AD FS) dağıtırken, Forms kimlik doğrulaması varsayılan olarak intranet için etkinleştirilmez. Windows tümleşik kimlik doğrulaması başarısız olursa, Forms kimlik doğrulaması kullanarak oturum açmanız istenir.

Bu sorunu çözmek için, Active Directory yerel kopyasının bulunduğu bilgisayarda AD FS Microsoft Yönetim Konsolu (MMC) ek bileşenini kullanarak Forms kimlik doğrulamasını etkinleştirin. Bunu yapmak için şu adımları uygulayın: 

1. Gezinti bölmesinde, **kimlik doğrulama ilkelerine**göz atın.
2. Ayrıntılar bölmesindeki **Eylemler** 'In altında **genel birincil kimlik doğrulamasını Düzenle**'yi seçin.
3. **Intranet** sekmesinde **Forms Authentication**öğesini seçin.
4. **Tamam 'ı** (veya **Uygula**) seçin.