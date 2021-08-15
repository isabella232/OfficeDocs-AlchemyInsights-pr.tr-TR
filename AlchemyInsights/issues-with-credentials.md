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
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986839"
---
# <a name="issues-with-credentials"></a>Kimlik bilgileriyle ilgili sorunlar

[Microsoft kimlik platformu ve OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) istemci kimlik bilgileri akışı, doğrudan OAuth 2.0 istemci kimlik bilgileri veri akışına karşı nasıl programla ilgili olduğunu açıklar.

**Uygulamanın parolasını veya sertifika kimlik bilgilerini nasıl yönetirim?**

Azure CLI'de az [ad](https://docs.microsoft.com/cli/azure/ad/app/credential) uygulama kimlik bilgilerini kullanarak uygulamanın parolasını veya sertifika kimlik bilgilerini silebilir, liste yerebilir veya sıfırlayabilirsiniz.

**Kullanıcılarım parolalarını nasıl sıfırlar?**

Kullanıcıların [parolalarını sıfırlaymadan önce](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) self servis parola sıfırlama için kaydolmaları gerekir. Bir kullanıcı kayıt olduktan sonra bu makaledeki yönergeleri izleyerek parolasını sıfırlayabilirsiniz: [İş veya okul parolanızı sıfırlama](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**Kullanıcılarım parolalarını nasıl değiştirir?**

Kullanıcılar bu makaledeki adımları kullanarak parolalarını değiştirebilir: [Parolanızı değiştirme](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Ayrıca, iki [aşamalı doğrulama için uygulama parolalarını yönetebilirler.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Kullanıcım parolasını değiştirirken veya sıfırlarken hata alıyor**

Bu bağlantı, kullanıcı parolasını sıfırlamaya çalışırken ortaya çıkabilecek yaygın sorunlar hakkında bilgi sağlar: [Yaygın sorunlar ve onların çözümleri](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Bir kullanıcının parolasını sıfırlamada sorunüyorum**

- Parolaları sıfırlama yetkiniz olduğundan emin olun. *Yalnızca genel parolalar ve kullanıcı yöneticileri kullanıcı parolalarını sıfırlar.* Genel yöneticiler ayrıca diğer ayrıcalıklı yönetici parolalarını da sıfırlar.

- Lisans gereksinimlerini anlıyoruz:

  - Kuruluşta en az bir lisans atanmış olması gerekir:
    - **Yalnızca bulut kullanıcıları** - Tüm Office 365 (O365) ücretli SKU veya Azure AD Basic
    - **Bulut ve/veya şirket içi kullanıcılar** - Azure AD Premium P1 veya P2, Enterprise Mobility + Security (EMS) veya Secure Productive Enterprise (SPE)
    - Lisans gereksinimleri hakkında daha fazla bilgi edinmek için bkz. Azure AD self servis [parola sıfırlama için lisans gereksinimleri.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Bir kullanıcının parolasını sıfırlamak için Azure AD'de kullanıcı bulun. Ardından, bu kullanıcıya ilişkin genel bakış blade'inde "parolayı sıfırla" düğmesine tıklayın.

**Parola sıfırlama düğmesi gri**

Bu kullanıcının parolalarını **sıfırlama yetkiniz** yok. *Yalnızca genel parolalar ve kullanıcı yöneticileri kullanıcı parolalarını sıfırlar.* Genel yöneticiler ayrıca diğer ayrıcalıklı yönetici parolalarını da sıfırlar.

**Parola sıfırlama blade'ini göremiyorum**

Parolaları sıfırlama yetkiniz yok. *Yalnızca genel parolalar ve kullanıcı yöneticileri kullanıcı parolalarını sıfırlar.* Genel yöneticiler ayrıca diğer ayrıcalıklı yönetici parolalarını da sıfırlar.

**Parola sıfırlamada şirket içi tümleştirme blade'ini göremiyorum**

- Şirket içi tümleştirme blade yalnızca karma ortamlarda görünür; yani şirket içi kullanıcının parolalarını işlemek için parola geri yazması kullanıyor olursanız.

- Aşağıdaki durumda bu blade'i görmüyorsanız:

  - Parola geri yazma kullanasınız
  - Parola geri yazma yükleme/bağlantınız ile ilgili bir sorun var
  - Azure AD bağlantı bağlantınız ile ilgili bir sorun Bağlan
  - Parola geri yazma ile ilgili sorunlar için daha fazla sorun giderme adımı için [bkz. Parola geri yazma sorunlarını giderme](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Bir kullanıcının parolasını nasıl sıfırla olduğumu bilmiyorum**

1. Uygun bir yönetici olarak Azure portalında oturum açın.
2. Kullanıcılar ve gruplar **blade'ine gidin,** Tüm **Kullanıcılar'ı seçin.**
3. Listeden bir kullanıcı seçin.
4. Seçili kullanıcı için Genel Bakış öğesini **seçin** ve komut çubuğundan Parolayı **sıfırla'yı seçin.**
5. Parolayı **sıfırla** düğmesini seçin ve ekrandaki yönergeleri izleyin.
    - Yalnızca Azure portal desteği parola **geri yazma işlemi** aracılığıyla gerçekleştirilen sıfırlamalar.

**Şirket içi kullanıcının parolasını Office 365 Admin portalında veya Office 365 uygulamasından sıfırladım ancak kullanıcı yine de oturum alamıyor**

Parola Geri Yazma bu portalda desteklenmiyor. Azure portalda kullanıcının parolasını yeniden sıfırlayın.
