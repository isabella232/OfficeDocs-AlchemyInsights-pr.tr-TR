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
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039986"
---
# <a name="problems-resetting-password"></a>Parola sıfırlama sorunları

Aşağıda, parolayı sıfırlarken karşılaşabilirsiniz bazı sorunlar ve olası çözümler ve yermektedir:

**Diğer kategorilerde yer alan parola sıfırlama ile ilgili bir sorun var**

- Parolaları sıfırlama yetkiniz olduğundan emin olun. Yalnızca genel parolalar ve kullanıcı yöneticileri kullanıcı parolalarını sıfırlar. Genel yöneticiler ayrıca diğer ayrıcalıklı yönetici parolalarını da sıfırlar.
- Lisans gereksinimlerini anlıyoruz:
    - Kuruluşta en az bir lisans atanmış
        - Yalnızca bulut kullanıcıları - Ücretli Office 365 (O365) SKU veya Azure AD Basic kullanıcıları
        - Bulut ve/veya şirket içi kullanıcılar - Azure AD Premium P1 veya P2, Enterprise Mobility + Security (EMS) veya Secure Productive Enterprise (SPE)
        - Lisans gereksinimleri hakkında daha fazla bilgi için Azure AD self servis parola sıfırlama için lisans [gereksinimleri makalesine bakın.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ayarlanıyorum parola sıfırlama ilkeyi test etmede sorunlanıyor**

- Son uygulanan ilkelerin tüm veri merkezlerine ve uç noktalara çoğaltılması birkaç dakika sürebilir. Veri merkezinden fiziksel mesafe, değişikliklerin ne kadar hızlı bir şekilde uygulandığını da etkiler.
- Küçük bir kullanıcı kümesiyle yöneticiyle değil, son kullanıcıyla ve pilotla test. Azure portalında yapılandırılan ilkeler yöneticilere değil YALNIZ ZAMAN son kullanıcılara uygulanır. Microsoft, herhangi bir Azure yönetici rolü için güçlü bir varsayılan iki sınırlı parola sıfırlama ilkesi zorlar (Örneğin: Genel Yönetici, Yardım masası Yöneticisi, Parola Yöneticisi, vb.)
    - Yöneticilere yönelik [ilkeler hakkında daha fazla bilgi öğrenin.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Parola sıfırlamayı dağıtmak istiyorum, ancak kullanıcılarımın ek güvenlik bilgilerini kaydetmelerini istemiyorum**

Kullanıcılarınız için verileri önceden doldurmak zorunda değildirler! - Yönetici olarak, parola sıfırlamayı kuruluşa göndermeden önce kullanıcılarınız için telefon ve e-posta özelliklerini ayarlayın. Bunu API, PowerShell veya Azure AD Veri Yönetimi Bağlan. Burada daha fazla bilgi edinebilirsiniz:
- [Kullanıcıların kaydolması gerekmeden parola sıfırlamayı dağıtma](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Parola sıfırlama ile kullanılan veriler](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Parola sıfırlama düğmesi gri**

Bu kullanıcının parolalarını sıfırlama yetkiniz yok. Yalnızca genel parolalar ve kullanıcı yöneticileri kullanıcı parolalarını sıfırlar. Genel yöneticiler ayrıca diğer ayrıcalıklı yönetici parolalarını da sıfırlar.

**Parola sıfırlama blade'ini göremiyorum**

Parolaları sıfırlama yetkiniz yok. Yalnızca genel parolalar ve kullanıcı yöneticileri kullanıcı parolalarını sıfırlar. Genel yöneticiler ayrıca diğer ayrıcalıklı yönetici parolalarını da sıfırlar.

**Parola sıfırlamada şirket içi tümleştirme blade'ini göremiyorum**

- Şirket içi tümleştirme blade yalnızca karma ortamlarda görünür; yani şirket içi kullanıcının parolalarını işlemek için parola geri yazması kullanıyor olursanız.
- Aşağıdaki durumda bu blade'i görmüyorsanız:
    - Parola geri yazma kullanasınız
    - Parola geri yazma yükleme/bağlantınız ile ilgili bir sorun var
    - Azure AD bağlantı bağlantınız ile ilgili bir sorun Bağlan
    - Parola geri yazma ile ilgili sorunlar için daha fazla sorun giderme adımı için Parola geri yazma [sorunlarını giderme bölümüne bakın.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Bir kullanıcının parolasını nasıl sıfırla olduğumu bilmiyorum**

1. Uygun bir yönetici olarak Azure portalında oturum açın.
1. Kullanıcılar ve gruplar blade'ine gidin, Tüm **Kullanıcılar'ı seçin.**
1. Listeden bir kullanıcı seçin.
1. Seçili kullanıcı için Genel Bakış öğesini **seçin** ve komut çubuğunda Parolayı sıfırla'ya **tıklayın.**
1. Ekrandaki yönergeleri izleyin.
    - Yalnızca Azure portal desteği parola geri yazma işlemi aracılığıyla gerçekleştirilen sıfırlamalar.

**Şirket içi kullanıcının parolasını Office 365 Admin portalında veya Office 365 uygulamasından sıfırladım ancak kullanıcı yine de oturum alamıyor**

Parola Geri Yazma bu portalda desteklenmiyor. Azure portalında kullanıcının parolasını yeniden sıfırlayın - portal.azure.com

