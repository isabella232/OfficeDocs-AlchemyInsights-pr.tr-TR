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
ms.openlocfilehash: 14f1454ad687b4d76cf419583b442685fa19b5a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321773"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>SMTP kimlik doğrulamasını ve sorun gidermeyi etkinleştirme

Bir posta kutusu için SMTP kimlik doğrulamasını etkinleştirmek veya Microsoft 365 ile bir cihaz veya uygulamanın kimlik doğrulaması gerçekleştirerek e-posta geçişi gerçekleştirerek e-postayı geçirerek 5.7.57 veya 5.7.3 veya 5.7.139 kodlu "Kimlik doğrulaması başarısız" veya "SmtpClientAuthentication" hatası alıyorsanız, sorunu çözmek için şu üç eylemi gerçekleştirin:

1. Güvenlik [varsayılanlarını hayır olarak etkinleştir'i](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) seçenek tarak Azure **güvenlik varsayılanlarını devre** dışı **bırak.**

    a. Güvenlik yöneticisi, Koşullu Erişim yöneticisi veya genel yönetici olarak Azure portalında oturum açın.<BR/>
    b. Azure Active Directory > **göz atabilirsiniz.**<BR/>
    c. Güvenlik **varsayılanlarını yönet'i seçin.**<BR/>
    d. Güvenlik **varsayılanlarını etkinleştir ayarını Hayır** olarak **ayarlayın.**<BR/>
    e. **Kaydet**'i seçin.

2. [Lisanslı posta kutusuna İstemci SMTP](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) gönderimi'ni etkinleştirin.

    a. Microsoft 365 yönetim merkezi'da Etkin **Kullanıcılar'a** gidin ve kullanıcısı seçin.<BR/>
    b. Posta sekmesine gidin ve E-posta **uygulamaları'nın altında E-posta** uygulamalarını **yönet'i seçin.**<BR/>
    d. Kimliği Doğrulanmış **SMTP'nin işaretli** olduğundan (etkinleştirildiğinden) emin olun.<BR/>
    e. Değişiklikleri **kaydet'i seçin.**<BR/>

3. [Lisanslı posta kutusunda Multi-Factor Authentication'ı (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) devre dışı bırakma.

    a. Gezinti Bölmesi'Microsoft 365 yönetim merkezi ve sol gezinti menüsünde Kullanıcılar Etkin **Kullanıcılar'ı**  >  **seçin.**<BR/>
    b. **Multi-factor authentication öğesini seçin.**<BR/>
    c. Kullanıcıyı seçin ve **Multi-Factorauth özelliğini devre dışı bırakma.**<BR/>
