---
title: 646 AADConnect biçimde nasıl yapılandırılır
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28317561"
---
# <a name="configure-sync-features"></a>Eşitleme özellikleri yapılandırma

Azure AD Bağlan varsayılan olarak etkin veya daha sonra etkinleştirmek üzere çeşitli özellikler içerir. Bazı özellikler belirli ortamlarda ek yapılandırma gerektirir.
  
- Azure AD için [filtreleme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) sınırları nesneler eşitlenir. Bilgisayar hesapları, varsayılan, tüm kullanıcılar, kişiler, gruplar ve Windows 10 tarafından eşitlenir. Ekleyebilir veya etki alanları, kuruluş birimleri veya diğer öznitelikleri temel nesneleri hariç tut. 
    
- [Parola karma eşitleme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) yerinde Active Directory'den Azure AD parola karma eşitler. Bu parola yönetimi tek bir yerde verir, ancak her ikisi de aynı parola kullanımını yerinde ve ortamlar bulut. Active Directory yetkili kaynak olduğu için kendi parola ilkelerini kullanabilirsiniz. 
    
- [Kendi kendine parola sıfırlama (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) hala yerinde, parola ilkesi uygulanırken bulut kendi parolalarını sıfırlamak kullanıcılar sağlar. 
    
- [Geri yazma aygıtı](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) Azure AD yerinde Active Directory'ye koşullu erişim için kullanılacak şekilde yeniden yazılması için kayıtlı aygıtlar sağlar. 
    
- [Silmeleri Engelle yanlışlıkla](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) çok fazla sayıda eşzamanlı nesne silme (eşitleme başına 500'den fazla nesneleri) önlemek için varsayılan olarak etkindir. Kuruluşunuzun gereksinimlerini karşılamak için bu ayarı değiştirebilirsiniz. 
    
- [Otomatik yükseltme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) hızlı yüklemeler için varsayılan olarak etkindir ve yardımcı Azure AD Bağlan sürümünüzün her zaman güncel olduğundan emin olun. 
    

