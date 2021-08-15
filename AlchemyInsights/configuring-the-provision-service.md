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
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033298"
---
# <a name="configuring-the-provision-service"></a>Sağlama hizmetini yapılandırma

Otomatik kullanıcı hazırlamanın çalışması için, Azure AD'nin İş Günü Web Hizmetleri API'sine bağlanmasına izin verecek geçerli kimlik bilgileri gerekir. Ayrıca, İşGünü'nden AD Kullanıcı Hazırlama uygulamasına kadar olan Test Bağlantısı düğmesi, Azure AD etki alanıyla ilişkilendirilmiş Azure AD Bağlan Sağlama Aracısı'ne bağlananın olup olduğunu da doğrular.

Azure portalı kimlik bilgilerini kaydetme sırasında hata döndür kaydediliyorsa, aşağıdaki önerilen adımları izleyin:

1. İşGünü'de tümleştirme sistemi kullanıcılarını yapılandırma öğretici bölümünde belirtildiği gibi İş Günü Tümleştirme Sistemi [Kullanıcı hesabını yapılandırmışsanız bunu onaylayın.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Azure AD Hizmet Bağlan Sağlama Aracı Hizmeti'nin, Hizmet Yönetim Konsolu'nu kullanarak şirket içi Windows sunucu üzerinde çalışır olduğunu onaylayın. Ayrıca, Şirket içi aracıları görüntüle düğmesine tıklayarak Azure portalında aracının durumunu da kontrol edebilirsiniz.
3. "İşGünü Kullanıcı Adı" alanına "Kiracı-adı" biçimini kullanarak değer username@workday emin olun. İşgünü kiracı adı yoksa İşgünü kimlik doğrulaması başarısız olur.
4. İşgünü uygulama kiracısı ile tümleştirmeyi yapılandırıyorsanız, İşgünü kiracının zamanlanmış kapalı kalma saatlerini notun. İşgünü, uygulama kiracılarının hafta sonları (çoğunlukla Cuma akşamdan Cumartesi sabahına kadar) kapalı zaman ayırıyor ve bu kapalı kalma süresi boyunca bağlantı hataları, uygulama kiracıları yeniden çevrimiçi olur noktada otomatik olarak çözülen bilinen bir sorundur.
5. Ender durumlarda, Kiracı yenilemesi nedeniyle Tümleştirme Sistemi Kullanıcısı'nın parolası değiştiyse veya hesabın kilitli ya da süresi dolmuşsa da bu hatayı alabilirsiniz. Lütfen İşgünü yöneticinizle Tümleştirme Sistemi kullanıcılarının durumunu kontrol edin.

Otomatik sağlama için iş günü yapılandırma hakkında daha fazla ayrıntı için bkz. [Öğretici: Otomatik kullanıcı sağlama için İşGünü'ne yapılandırma.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
