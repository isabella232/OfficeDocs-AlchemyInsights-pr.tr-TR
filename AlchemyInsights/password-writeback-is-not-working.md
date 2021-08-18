---
title: Parola Geri Yazma çalışmıyor
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324943"
---
# <a name="password-writeback-is-not-working"></a>Parola Geri Yazma çalışmıyor

**Parola geri dönüşlerini yapılandırmada sorunm var**

- Parola geri yazma, birinci sınıf bir özelliktir.
- Lisans gereksinimlerini anlıyoruz:
  - Kuruluşta en az bir lisans atanmış
  - **Yalnızca bulut kullanıcıları** - Tüm Office 365 (O365) ücretli SKU veya Azure AD Basic
  - **Bulut ve/veya şirket içi kullanıcılar** - Azure AD Premium P1 P2, Enterprise Mobility + Security (EMS) veya Secure Productive Enterprise (SPE)
    - Lisans gereksinimleri hakkında daha fazla bilgi edinmek için bkz. Azure AD self servis [parola sıfırlama için lisans gereksinimleri](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- En az bir yönetici hesabınız ve uygun lisanslardan birinin olduğu bir test kullanıcı hesabınız var.
- Parola geri yazmanın çalışması Bağlan için Azure AD Emulator'i Birincil Etki Alanı Denetleyicisi'ne bağlamanız gerekir. Active Directory eşitleme bağlayıcısı özelliklerine Bağlan tıklayın ve dizin  bölümlerini yapılandır öğesini seçerek Azure AD Bağlan'i Birincil Etki Alanı Denetleyicisi'nin **kullanımını yapılandırabilirsiniz.** Orada, etki alanı denetleyicisi bağlantı **ayarları bölümünü bakın** ve yalnızca tercih edilen etki alanı denetleyicilerinin kullanımı başlıklı kutuyu **işaretleyin.**
    **Not:Tercih** edilen DC bir PDC öykünücüsü değil, Azure AD Bağlan parola geri yazma için PDC'ye ulaşmaya devam eder.
- Kiracınız parola sıfırlama yapılandırılmış ve etkinleştirilmiştir. Daha fazla bilgi için [bkz. Kullanıcıların Azure AD parolalarını sıfırlamalarını etkinleştirme](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Parola Geri Yazma'nın etkinleştirilen yönetici hesabının bir bulut yöneticisi hesabı olduğundan emin olun (şirket içi AD'de değil Azure AD'de oluşturulur)
- En son hizmet paketleri yüklü olan Windows Server 2008 R2, Windows Server 2012 veya Windows Server 2012 R2 çalıştıran tek veya çok ormanlı bir AD şirket içi dağıtımınız var
- Azure AD Bağlan aracı yüklü ve AD ortamınızı buluta eşitleme için hazırladınız. Parola geri yazma işlemini sınamadan önce, önce Hem AD'den hem de Azure AD'den Azure AD veya Azure AD'den tam içeri aktarma ve tam eşitleme Bağlan.
- Daha fazla bilgi edinmek için Bkz. [Azure AD'de](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations) tam eşitleme ve tam içeri aktarma Bağlan

**Parola geri yazma bağlantısıyla ilgili bir sorun var**

1. Azure AD Bağlan'in en [son sürümünü indirme ve etkinleştirme](https://www.microsoft.com/download/details.aspx?id=47594)
2. Güvenlik duvarı yapılandırması: Azure AD Bağlan (1.1.443 ve üzeri), aşağıdakilere giden **HTTPS** erişimi gerekir:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Boşta kalma bağlantılarının en az 2-3 dakika kalıcı olmasına izin ver

**Parola geri yazma ile ilgili sorun halen devam ediyor**

- Hala sorun yaşıyorsanız, Azure AD Posta Hizmeti aracında parola geri yazma hizmetini devre dışı bırakmayı ve yeniden Bağlan deneyin
- Daha fazla bilgi edinmek için bkz. Parola geri yazma özelliğini [devre dışı bırakma ve yeniden etkinleştirme](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
