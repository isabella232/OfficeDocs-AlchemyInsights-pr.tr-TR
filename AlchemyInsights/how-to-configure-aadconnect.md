---
title: 646 AADConnect nasıl yapılandırılatır
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722583"
---
# <a name="configure-sync-features"></a>Eşitleme özelliklerini yapılandırma

Azure AD Connect varsayılan olarak etkinleştirilen veya daha sonra etkinleştirebileceğiniz birkaç özellik içerir. Bazı özellikler belirli ortamlarda ek yapılandırma gerektirir.

- [Filtreleme,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) nesnelerin Azure AD ile eşitlenerek sınırlandırılmalarını sınırlar. Varsayılan olarak, tüm kullanıcılar, kişiler, gruplar ve Windows 10 bilgisayar hesapları eşitlenir. Etki alanlarına, BIZE veya diğer özniteliklere dayalı nesneleri içerebilir veya hariç tutabilirsiniz.

- [Parola karma eşitleme,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) şirket içi Active Directory'den Azure AD'ye parola karmasını eşitler. Bu, parola yönetiminin tek bir konumda yapılmasına izin verir, ancak hem şirket içinde hem de bulut ortamlarında aynı parolanın kullanılmasına olanak tanır. Etkin Dizin yetkili kaynak olduğundan, kendi parola ilkelerinizi kullanabilirsiniz.

- [Self servis parola sıfırlama (SSPR),](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) kullanıcıların şirket içi parola ilkenizi uygularken bulutta kendi parolalarını sıfırlamalarına olanak tanır.

- [Aygıt geri yüklemesi,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) Azure AD'deki kayıtlı aygıtların şirket içi Active Directory'ye yazılmasına izin verir, böylece koşullu erişim için kullanılabilirler.

- Çok fazla eşzamanlı nesne silme (eşitleme başına 500'den fazla nesne) önlemeye yardımcı olmak için varsayılan olarak [yanlışlıkla silmeleri](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) önlemek. Kuruluşunuzun gereksinimlerini karşılamak için bu ayarı değiştirebilirsiniz.

- [Otomatik yükseltme,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) ekspres yüklemeler için varsayılan olarak etkinleştirilir ve Azure AD Connect sürümünün her zaman geçerli olmasını sağlamaya yardımcı olur.
