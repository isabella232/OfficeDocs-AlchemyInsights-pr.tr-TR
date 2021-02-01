---
title: Kimlik bilgileriyle ilgili sorunlar
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063722"
---
# <a name="issues-with-credentials"></a>Kimlik bilgileriyle ilgili sorunlar

[Microsoft kimlik platformu ve OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) istemci kimlik bilgileri akışı, doğrudan OAuth 2.0 istemci kimlik bilgileri erişim akışına karşı nasıl programlanacaklarını açıklar.

**Uygulamanın parolasını veya sertifika kimlik bilgilerini nasıl yönetirim?**

Azure CLI'de, bir [uygulamanın parolasını veya](https://docs.microsoft.com/cli/azure/ad/app/credential) sertifika kimlik bilgilerini silmek, listele veya sıfırlamak için az ad uygulaması kimlik bilgilerini kullanabilirsiniz.

**Kullanıcılarım parolalarını nasıl sıfırlar?**

Kullanıcıların [parolalarını sıfırlayamadan önce self](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) servis parola sıfırlama için kaydolmaları gerekir. Kullanıcı kayıt olduktan sonra bu makaledeki yönergeleri izleyerek parolasını sıfırlayabilirsiniz: [İş veya okul parolanızı sıfırlayın.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Kullanıcılarım parolalarını nasıl değiştirir?**

Kullanıcılar bu makaledeki adımları kullanarak parolalarını değiştirebilir: [Parolanızı değiştirme.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Ayrıca, iki [aşamalı doğrulama için uygulama parolalarını da yönetebilirler.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Kullanıcım parolasını değiştirirken veya sıfırlarken hata alıyor**

Bu bağlantı, kullanıcı parolasını sıfırlamaya çalışırken ortaya çıkabilecek yaygın sorunlar hakkında bilgi sağlar: Sık karşılaşılan [sorunlar ve onların çözümleri](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Kullanıcının parolasını sıfırlamayla ilgili bir sorun var**

- Parolaları sıfırlama yetkiniz olduğundan emin olun. *Kullanıcı parolalarını yalnızca genel parolalar ve kullanıcı yöneticileri sıfırlar.* Genel yöneticiler, diğer ayrıcalıklı yönetici parolalarını da sıfırlar.

- Lisans gereksinimlerini anlayalın:

  - Kuruluşta en az bir lisans atanmış olması gerekir:
    - **Yalnızca bulut kullanıcıları** - Ücretli tüm Office 365 (O365) SKU'ları veya Azure AD Basic
    - **Bulut ve/veya şirket içi** kullanıcılar - Azure AD Premium P1 veya P2, Enterprise Mobility + Security (EMS) veya Secure Productive Enterprise (SPE)
    - Lisans gereksinimleri hakkında daha fazla bilgi edinmek için, Azure AD self servis parola sıfırlama [lisans gereksinimlerine bakın.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Kullanıcının parolasını sıfırlamak için, Azure AD'de bir kullanıcı bulun. Ardından, söz alan kullanıcıya genel bakış blade'inde "parolayı sıfırla" düğmesine tıklayın.

**Parola sıfırlama düğmesi gri**

Bu kullanıcının parolalarını **sıfırlama yetkiniz** yok. *Kullanıcı parolalarını yalnızca genel parolalar ve kullanıcı yöneticileri sıfırlar.* Genel yöneticiler, diğer ayrıcalıklı yönetici parolalarını da sıfırlar.

**Parola sıfırlama blade'ini göremiyorum**

Parolaları sıfırlama yetkiniz yok. *Kullanıcı parolalarını yalnızca genel parolalar ve kullanıcı yöneticileri sıfırlar.* Genel yöneticiler, diğer ayrıcalıklı yönetici parolalarını da sıfırlar.

**Parola sıfırlamada şirket içi tümleştirme blade'ini göremiyorum**

- Şirket içi tümleştirme blade yalnızca karma ortamlarda görüntülenir; yani şirket içi kullanıcının parolalarını işlemek için parola geri yazma kullanıyor olursanız.

- Şu durumda bu blade'i görmüyorsanız:

  - Parola geri yazma kullanasınız
  - Parola geri yazma işleminin yükleme/bağlantısı ile ilgili bir sorun var
  - Azure AD Connect'in yükleme/bağlantısı ile ilgili bir sorun var
  - Parola geri yazma ile ilgili sorunlar için daha fazla sorun giderme adımı için bkz. [Parola geri yazma sorunlarını giderme](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Bir kullanıcının parolasını nasıl sıfırlay bilmiyorum**

1. Uygun bir yönetici olarak Azure portalında oturum açın.
2. Kullanıcılar ve gruplar **blade'ine gidin,** Tüm **Kullanıcılar'ı seçin.**
3. Listeden bir kullanıcı seçin.
4. Seçili kullanıcı için Genel **Bakış'ı seçin** ve sonra komut çubuğunda Parolayı **sıfırla'yı seçin.**
5. Parolayı **sıfırla** düğmesini seçin ve ekrandaki yönergeleri izleyin.
    - Yalnızca Azure portal desteği ile **gerçekleştirilen sıfırlamalar** parola geri yazma işlemidir.

**Şirket içi kullanıcı parolasını Office 365 Yönetim portalında veya Office 365 mobil uygulamasından sıfırlayam, ancak kullanıcı yine de oturum ala**

Parola Geri Yazma bu portalda desteklenmiyor. Azure portalda kullanıcının parolasını yeniden sıfırlayın.
