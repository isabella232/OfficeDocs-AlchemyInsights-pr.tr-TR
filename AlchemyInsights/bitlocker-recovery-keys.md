---
title: BitLocker kurtarma anahtarları
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
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685906"
---
# <a name="accessing-bitlocker-recovery-keys"></a>BitLocker Kurtarma anahtarlarına erişme

BitLocker ayarları Intune Endpoint Protection Ilkesini yapılandırırken, BitLocker kurtarma bilgilerinin Azure Active Directory 'de depolanması gerekip gerekmediği tanımlanır.

Bu ayar yapılandırılırsa, cihaz için depolanan kurtarma verileri Intune cihazlarındaki verilerin iki yolu nedeniyle bir Intune yöneticisine görünür olmalıdır:

Cihazlar-Azure AD cihazları-> "aygıt" veya cihazlar-> tüm cihazlar-> "cihaz"-> kurtarma anahtarları

Alternatif olarak, cihaza yönetimsel erişim varsa, kurtarma anahtarı (parola) yükseltilmiş bir komut isteminden aşağıdaki komut çalıştırılarak görülebilir:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Cihaz Intune 'da kaydolma öncesinde şifrelendiyse, kurtarma anahtarı, OOBE işlemi sırasında cihazda oturum açmak için kullanılan "Microsoft hesabı" (MSA) ile ilişkilendirilmiş olabilir. Öyleyse,  https://onedrive.live.com/recoverykey Bu MSA ile erişilmesi ve oturum açmak, kurtarma anahtarlarının depolandığı cihazları göstermelidir.
 
Cihaz, etki alanı tabanlı Grup İlkesi aracılığıyla yapılandırma sonucunda şifrelenmişse, kurtarma bilgileri şirket içi Active Directory 'de depolanabilir.
 

