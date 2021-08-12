---
title: SMTP kimlik doğrulamasını ve sorun gidermeyi etkinleştirme
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: f6f0228f6cdf7e07c9f439c54a7a2bd5364381c0e47dc80117bd964c5eafea61
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957228"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>SMTP kimlik doğrulamasını ve sorun gidermeyi etkinleştirme

Bir posta kutusu için SMTP kimlik doğrulamasını etkinleştirmek veya Microsoft 365 ile bir cihaz veya uygulamanın kimlik doğrulaması gerçekleştirerek e-posta geçişi gerçekleştirerek geçiş yapmaya çalışmanız sırasında 5.7.57 veya 5.7.3 veya 5.7.139 kodlu "İstemci kimliği doğrulanmadı", "Kimlik doğrulaması başarısız" veya "SmtpClientAuthentication" hatası alıyorsanız, sorunu çözmek için şu üç eylemi gerçekleştirin:

1. Güvenlik [varsayılanlarını hayır olarak etkinleştir'i](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) seçenek tarak Azure **güvenlik varsayılanlarını devre** dışı **bırak.**

    a. Güvenlik yöneticisi, Koşullu Erişim yöneticisi veya genel yönetici olarak Azure portalında oturum açın.<BR/>
    b. Azure Active Directory > **göz atabilirsiniz.**<BR/>
    c. Güvenlik **varsayılanlarını yönet'i seçin.**<BR/>
    d. Güvenlik **varsayılanlarını etkinleştir ayarını Hayır** olarak **ayarlayın.**<BR/>
    e. **Kaydet**'i seçin.

2. [Lisanslı posta kutusuna İstemci SMTP](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) gönderimi'ni etkinleştirin.

    a. Arama Microsoft 365 yönetim merkezi, Etkin **Kullanıcılar'a gidin** ve kullanıcısı seçin.<BR/>
    b. Posta sekmesine gidin ve E-posta **uygulamaları'nın altında E-posta** uygulamalarını **yönet'i seçin.**<BR/>
    d. Kimliği Doğrulanmış **SMTP'nin işaretli** olduğundan (etkinleştirildiğinden) emin olun.<BR/>
    e. Değişiklikleri **kaydet'i seçin.**<BR/>

3. [Lisanslı posta kutusunda Multi-Factor Authentication'ı (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) devre dışı bırakma.

    a. Gezinti Bölmesi'Microsoft 365 yönetim merkezi ve sol gezinti menüsünde Kullanıcılar Etkin **Kullanıcılar'ı**  >  **seçin.**<BR/>
    b. **Multi-factor authentication öğesini seçin.**<BR/>
    c. Kullanıcıyı seçin ve **Multi-Factorauth özelliğini devre dışı bırakma.**<BR/>
