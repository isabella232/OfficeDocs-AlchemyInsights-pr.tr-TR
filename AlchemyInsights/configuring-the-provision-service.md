---
title: Sağlama hizmetini yapılandırma
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484047"
---
# <a name="configuring-the-provision-service"></a>Sağlama hizmetini yapılandırma

Otomatik kullanıcı sağlamanın çalışması için, Azure AD'nin İşGünü Web Hizmetleri API'sine bağlanmasını sağlayan geçerli kimlik bilgileri gerekir. Ayrıca, İşGünü'nden AD Kullanıcı Hazırlama uygulamasına yönelik Test Bağlantısı düğmesi, AD Etki Alanı ile ilişkilendirilmiş Azure AD Connect Sağlama Aracısına bağlananın mümkün olup olduğunu da doğrular.

Azure portalı kimlik bilgilerini kaydettikten sonra hata döndür kaydediliyorsa, aşağıdaki önerilen adımları izleyin:

1. İşGünü'de tümleştirme sistemi kullanıcılarını yapılandırma öğretici bölümünde belirtildiği gibi İşGünü Tümleştirme Sistemi Kullanıcı hesabını [yapılandırmış olduğunu onaylayın.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Hizmetler Yönetim Konsolu'nu kullanarak şirket içi Windows sunucunuzda Azure AD Connect Sağlama Aracı Hizmeti'nin çalışır ve çalışır olduğunu onaylayın. Ayrıca, Şirket içi aracıları görüntüle düğmesine tıklayarak Azure portalında aracının durumunu da kontrol edebilirsiniz.
3. Kiracı-adı biçimini kullanarak "İşGünü Kullanıcı Adı" alanı değerini username@workday emin olun. İşgünü kiracı adı yoksa, İşGünü kimlik doğrulaması başarısız olur.
4. İşGünü uygulama kiracısı ile tümleştirmeyi yapılandırıyorsanız, İşGünü kiracınıza yönelik zamanlanmış kapalı kalma saatlerini not edersiniz. İşgünü, uygulama kiracıları için hafta sonları (çoğunlukla Cuma akşamdan Cumartesi sabahına kadar) zamanlanmış ve bu kesinti süresi boyunca bağlantı hataları, uygulama kiracıları yeniden çevrimiçi olur dönmez otomatik olarak çözülen bilinen bir sorundur.
5. Ender durumlarda, Tümleştirme Sistemi Kullanıcısı parolasının kiracı yenilemesi nedeniyle değişmesi veya hesabın kilitli veya süresinin dolması durumu nedeniyle bu hatayı da alabilirsiniz. Lütfen İşGünü yöneticinizle Tümleştirme Sistemi kullanıcılarının durumunu kontrol edin.

Otomatik sağlama için iş günü yapılandırma hakkında daha fazla ayrıntı için öğreticiye bakın: Otomatik kullanıcı [sağlama için İşGünü'ne yapılandırma.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
