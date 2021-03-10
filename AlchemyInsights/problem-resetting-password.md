---
title: Parola sıfırlama sorunu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696281"
---
# <a name="problems-resetting-password"></a>Parola sıfırlama sorunları

Parolayı sıfırlarken karşılaş olabileceğiniz sorunlardan bazıları ve olası çözümler aşağıda ve aşağıda ve listelerde yer alan bazı sorunlar yermektedir:

**Parola sıfırlama ile ilgili diğer kategorilerde yer alan bir sorun var**

- Parolaları sıfırlama yetkiniz olduğundan emin olun. Kullanıcı parolalarını yalnızca genel parolalar ve kullanıcı yöneticileri sıfırlar. Genel yöneticiler, diğer ayrıcalıklı yönetici parolalarını da sıfırlar.
- Lisans gereksinimlerini anlamadan emin olun:
    - Kuruluşta en az bir lisans atanmış olması gerekir
        - Yalnızca bulut kullanıcıları - Ücretli tüm Office 365 (O365) SKU'ları veya Azure AD Basic
        - Bulut ve/veya şirket içi kullanıcılar - Azure AD Premium P1 veya P2, Enterprise Mobility + Security (EMS) veya Secure Productive Enterprise (SPE)
        - Lisans gereksinimleri hakkında daha fazla bilgi için, Azure AD self servis parola sıfırlama lisans [gereksinimleri makalesine bakın.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Parola sıfırlama ilkemi test etmede sorunm var**

- Son uygulanan ilkelerin tüm veri merkezlerine ve uç noktalara çoğaltılması birkaç dakika sürebilir. Veri merkezinden fiziksel uzaklık da değişikliklerin ne kadar hızlı uygulandığını etkiler.
- Küçük bir kullanıcı kümesiyle yönetici değil son kullanıcıyla test ve pilot uygulama. Azure portalında yapılandırılan ilkeler yöneticilere değil YALNIZLIK son kullanıcılara uygulanır. Microsoft, herhangi bir Azure yönetici rolü için güçlü bir varsayılan iki kapılı parola sıfırlama ilkesi zorunlur (Örnek: Genel Yönetici, Yardım Masası Yöneticisi, Parola Yöneticisi, vb.)
    - Yöneticilere yönelik [ilkeler hakkında daha fazla bilgi.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Parola sıfırlamayı dağıtmak istiyorum, ancak kullanıcılarımı ek güvenlik bilgilerini kaydetmelerini istemiyorum**

Kullanıcılarınız için verileri önceden doldurmak zorunda değil! - Bir yönetici olarak, parola sıfırlamayı kuruluşa göndermeden önce kullanıcılarınız için telefon ve e-posta özelliklerini ayarlayabilirsiniz. Bunu API, PowerShell veya Azure AD Connect kullanarak da kullanabilirsiniz. Buradan daha fazla bilgi edinebilirsiniz:
- [Kullanıcıların kaydolması gerekmeden parola sıfırlamayı dağıtma](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Parola sıfırlama ile kullanılan veriler](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Parola sıfırlama düğmesi gri**

Bu kullanıcının parolalarını sıfırlama yetkiniz yok. Kullanıcı parolalarını yalnızca genel parolalar ve kullanıcı yöneticileri sıfırlar. Genel yöneticiler, diğer ayrıcalıklı yönetici parolalarını da sıfırlar.

**Parola sıfırlama blade'ini göremiyorum**

Parolaları sıfırlama yetkiniz yok. Kullanıcı parolalarını yalnızca genel parolalar ve kullanıcı yöneticileri sıfırlar. Genel yöneticiler, diğer ayrıcalıklı yönetici parolalarını da sıfırlar.

**Parola sıfırlamada şirket içi tümleştirme blade'ini göremiyorum**

- Şirket içi tümleştirme blade yalnızca karma ortamlarda görüntülenir; yani şirket içi kullanıcının parolalarını işlemek için parola geri yazma kullanıyor olursanız.
- Şu durumda bu blade'i görmüyorsanız:
    - Parola geri yazma kullanasınız
    - Parola geri yazma işleminin yükleme/bağlantısı ile ilgili bir sorun var
    - Azure AD Connect'in yükleme/bağlantısı ile ilgili bir sorun var
    - Parola geri yazma ile ilgili sorunlar için daha fazla sorun giderme adımı için Parola geri yazma [sorunlarını giderme bölümüne bakın](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Bir kullanıcının parolasını nasıl sıfırlay bilmiyorum**

1. Uygun bir yönetici olarak Azure portalında oturum açın.
1. Kullanıcılar ve gruplar blade'ine gidin, Tüm **Kullanıcılar'ı seçin.**
1. Listeden bir kullanıcı seçin.
1. Seçili kullanıcı için Genel **Bakış'ı seçin** ve sonra komut çubuğunda Parolayı sıfırla'ya **tıklayın.**
1. Ekrandaki yönergeleri izleyin.
    - Yalnızca Azure portal desteği ile gerçekleştirilen sıfırlamalar parola geri yazma işlemidir.

**Şirket içi kullanıcı parolasını Office 365 Yönetim portalında veya Office 365 mobil uygulamasından sıfırlayam, ancak kullanıcı yine de oturum ala**

Parola Geri Yazma bu portalda desteklenmiyor. Azure portalında kullanıcının parolasını yeniden sıfırlama - portal.azure.com

