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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243732"
---
# <a name="password-writeback-is-not-working"></a>Parola Geri Yazma çalışmıyor

**Parola geri yazma yapılandırmada sorunm var**

- Parola geri yazma, premium bir özelliktir.
- Lisans gereksinimlerini anlamadan emin olun:
  - Kuruluşta en az bir lisans atanmış olması gerekir
  - **Yalnızca bulut kullanıcıları** - Ücretli tüm Office 365 (O365) SKU'ları veya Azure AD Basic
  - **Bulut ve/veya şirket içi** kullanıcılar - Azure AD Premium P1 veya P2, Enterprise Mobility + Security (EMS) veya Secure Productive Enterprise (SPE)
    - Lisans gereksinimleri hakkında daha fazla bilgi edinmek için, Azure AD self servis parola sıfırlama [lisans gereksinimlerine bakın](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- En az bir yönetici hesabınız ve uygun lisanslardan birini olan bir test kullanıcı hesabınız var.
- Parola geri yazmanın çalışması için Azure AD Connect'i Birincil Etki Alanı Denetleyicisi Öykünücüsü'ne bağlamanız gerekir. Active Directory eşitleme bağlayıcısı özelliklerine sağ tıklayarak ve  ardından dizin bölümlerini yapılandır seçeneğini seçerek, Azure AD Connect'i Birincil Etki Alanı Denetleyicisi'nden kullanmak **üzere yapılandırabilirsiniz.** Buradan, etki alanı denetleyicisi **bağlantı ayarları bölümünü** bakın ve yalnızca tercih edilen etki alanı denetleyicilerinin kullanımı başlıklı kutuyu **işaretleyin.**
  > [!NOTE]
  > Tercih edilen DC bir PDC öykünücüsü değilse, Azure AD Connect parola geri yazma için PDC'ye ulaşmaya devam eder.
- Parola sıfırlama kiracınız içinde yapılandırıldı ve etkinleştirildi. Daha fazla bilgi için [bkz. Kullanıcıların Azure AD parolalarını sıfırlamalarını etkinleştirme.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Parola Geri Yazma'nın etkinleştirmek için kullanılan yönetici hesabının bir bulut yöneticisi hesabı olduğundan emin olun (şirket içi AD'de değil Azure AD'de oluşturulur)
- En son hizmet paketlerinin yüklü olduğu Windows Server 2008 R2, Windows Server 2012 veya Windows Server 2012 R2 çalıştıran tek veya çok ormanlı bir AD şirket içi dağıtımınız var
- Azure AD Connect aracı yüklü ve AD ortamınızı bulutla eşitleme için hazırladınız. Parola geri yazma işlemini sınamadan önce, Azure AD Connect'te hem AD'den hem de Azure AD'den tam içeri aktarma ve tam eşitlemeyi tamamlayamadan önce emin olun.
- Daha fazla bilgi edinmek için [Azure AD Connect'te tam eşitleme ve tam içeri aktarma yapmayı öğrenin](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Parola geri yazma bağlantısıyla ilgili bir sorun var**

1. [Azure AD Connect'in](https://www.microsoft.com/download/details.aspx?id=47594) en son sürümünü indirme ve etkinleştirme
2. Güvenlik duvarı yapılandırması: Azure AD Connect aracının (1.1.443 ve üzeri) aşağıdakilere giden **HTTPS** erişimi olması gerekir:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Boşta bağlantının en az 2-3 dakika kalıcı olmasına izin ver

**Parola geri yazma sorunlarım devam ediyor**

- Hala sorun yaşıyorsanız, Azure AD Connect aracında parola geri yazma hizmetini devre dışı bırakmayı ve yeniden etkinleştirmeyi deneyin
- Daha fazla bilgi edinmek için parola geri [yazma özelliğini devre dışı bırakmayı ve yeniden etkinleştirmeyi öğrenin](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
