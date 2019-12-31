---
title: Bitlocker kurtarma tuşları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908834"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Bitlocker kurtarma tuşlarına erişim

Bitlocker ayarlarını Intune Endpoint Protection İlke'yi yapılandırırken, Bitlocker kurtarma bilgilerinin Azure Etkin Dizini'nde depolanıp depolanmayacağını tanımlamak mümkündür.

Bu ayar yapılandırılırsa, depolanan kurtarma verileri, Intune Devices bıtırcı bıçaktaki aygıt kaydı verilerinin bir parçası olarak bir Intune yöneticisi tarafından iki şekilde görülebilir:

Cihazlar - Azure AD aygıtları -> "Aygıt" VEYA Aygıtlar -tüm cihazlar > -> "Aygıt" -> Kurtarma tuşları

Alternatif olarak, aygıtın kendisine yönetimsel erişim varsa, kurtarma anahtarı (Parola) yükseltilmiş bir komut isteminden aşağıdaki komutu çalıştırarak görülebilir:

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
Aygıt Intune'a kaydolmadan önce şifrelenmişse, kurtarma anahtarı OOBE işlemi sırasında aygıtta oturum açmada kullanılan "Microsoft Hesabı" (MSA) ile ilişkilendirilmiş olabilir. Bu durumda, msa https://onedrive.live.com/recoverykey ile erişim ve oturum açma, kurtarma anahtarlarının depolandığı aygıtları göstermelidir.
 
Aygıt etki alanı tabanlı grup ilkesi aracılığıyla yapılandırma sonucunda şifrelenmişse, kurtarma bilgileri şirket içi Etkin Dizinde depolanabilir.
 

