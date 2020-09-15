---
title: 646 AADConnect 'i yapılandırma
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
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704509"
---
# <a name="configure-sync-features"></a>Eşitleme özelliklerini yapılandırma

Azure AD Connect, varsayılan olarak etkinleştirilen veya daha sonra etkinleştirebileceğiniz çeşitli özellikler içerir. Bazı özellikler belirli ortamlarda ek yapılandırma gerektirir.

- [Filtreleme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) sınırları nesneler Azure AD ile eşitlenir. Varsayılan olarak, tüm kullanıcılar, kişiler, gruplar ve Windows 10 bilgisayar hesapları eşitlenir. Etki alanları, kuruluş birimleri veya diğer özniteliklere göre nesneleri ekleyebilir veya dışlayabilirsiniz.

- [Parola karması eşitleme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) , parola karmasını şirket Içi Active Directory 'den Azure AD 'ye eşitler. Bu, tek bir konumda parola yönetimine olanak tanır, ancak şirket içi ve bulut ortamlarında aynı parolanın kullanılmasını sağlar. Active Directory, yetkili kaynak olduğundan, kendi parola ilkelerinizi kullanabilirsiniz.

- [Self servis parola sıfırlama (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) , şirket içi parola ilkenizi uygularken kullanıcıların kendi parolalarını kendi parolalarını sıfırlamalarına olanak tanır.

- [Cihaz geri yazma](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) , Azure AD 'deki kaydettirilmiş cihazların, şirket Içi Active Directory 'ye geri yazılmasına olanak tanır, böylece koşullu erişim için kullanılabilir.

- Çok sayıda eşzamanlı nesne silme işlemi yapılmasını engellemeye yardımcı olmak için [yanlışlıkla silme Işlemlerini önleyin](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) (eşitleme başına 500 nesnelerden fazla). Kuruluşunuzun gereksinimlerini karşılayacak şekilde bu ayarı değiştirebilirsiniz.

- [Otomatik yükseltme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) , hızlı yüklemeler için varsayılan olarak etkinleştirilir ve Azure AD Connect sürümünüzün her zaman güncel olmasını sağlamaya yardımcı olur.
