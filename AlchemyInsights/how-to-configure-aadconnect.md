---
title: 646 AADConnect'i yapılandırma
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963663"
---
# <a name="configure-sync-features"></a>Eşitleme özelliklerini yapılandırma

Azure AD Bağlan varsayılan olarak etkinleştiren veya daha sonra etkinleştirebilirsiniz çeşitli özellikler içerir. Bazı özellikler belirli ortamlarda ek yapılandırma gerektirir.

- [Filtreleme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) sınırları nesneleri Azure AD ile eşitlenir. Varsayılan olarak, tüm kullanıcılar, kişiler, gruplar Windows 10 bilgisayar hesapları eşitlenir. Nesneleri etki alanları, OUs veya diğer özniteliklere dayalı olarak dahil edin veya hariç tutabilirsiniz.

- [Parola karması eşitlemesi,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) parola karmasını şirket içi Active Directory'den Azure AD'ye eşitler. Bu, tek konumda parola yönetimine olanak tanır, ancak aynı parolanın hem şirket içi hem de bulut ortamlarında kullanımına izin verir. Yetkili kaynak Active Directory olduğundan, kendi parola ilkelerinizi kullanabilirsiniz.

- [Self servis parola sıfırlama (SSPR),](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) kullanıcıların bulutta kendi parolalarını sıfırlamalarına ve bu sırada şirket içi parola ilkenizi uygulamaya devam etmelerine olanak sağlar.

- [Cihaz geri yazma](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) özelliği, Azure AD'de kayıtlı cihazların şirket içi Active Directory'ye geri yazarak koşullu erişim için kullanılabilirlerini sağlar.

- [Çok fazla eşzamanlı nesne silme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) işlemini (eşitleme başına 500'den fazla nesne) önlemeye yardımcı olmak için, varsayılan olarak yanlışlıkla silmeleri önle etkindir. Bu ayarı, kuruma uygun olarak değiştirebilirsiniz.

- [Hızlı yüklemelerde](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) otomatik yükseltme varsayılan olarak etkindir ve Azure AD kullanıcı sürümünizin her zaman güncel Bağlan yardımcı olur.
