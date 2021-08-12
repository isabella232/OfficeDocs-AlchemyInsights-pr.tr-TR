---
title: 451 4.7.0 Geçici sunucu hatası. Lütfen daha sonra yeniden deneyin. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812593"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Geçici sunucu hatası. Lütfen daha sonra yeniden deneyin. PRX4

SMTP İstemci Gönderimi yöntemini kullanarak Smarthost "smtp.office365.com" üzerinden e-posta gönderirken bir sorun ile karşılaşabilirsiniz ve şu hatayı alabilirsiniz: "451 4.7.0 Geçici sunucu hatası. Lütfen daha sonra yeniden deneyin. PRX4 çoğunlukla geçicidir." 

SMTP istemci gönderimi için paylaşılan posta kutusu kullanmamanızı sağlar çünkü SMTP istemci Gönderimi yöntemi posta göndermek için lisanslı bir posta kutusu gerektirir. Bununla birlikte, paylaşılan bir posta kutusu kullanıyorsanız ve sorun devam ediyorsa, şunları kontrol edin:

1. Şu PowerShell komutunu çalıştırarak kullanılan lisanslı posta kutusunda İstemci SMTP gönderimi'ni etkinleştirin:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    VEYA

    1. Etkin kullanıcılar Microsoft 365 yönetim merkezi > **gidin** ve kullanıcısı seçin.
    1. E-posta uygulamaları'> **posta uygulamaları'>** e-posta **uygulamalarını yönet'i seçin.** 
    1. Kimliği Doğrulanmış **SMTP ayarının işaretli** olduğundan (etkinleştirildiğinden) emin olun.
    1. Değişiklikleri **kaydet'i seçin.**
    
    Kuruluşun tamamı için SMTP Kimlik Doğrulamasını etkinleştirmek için şu komutu çalıştırın:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Not:** Güvenlik nedenleriyle, yalnızca kullanılan posta kutusu için SMTP Kimlik Doğrulamasını etkinleştirmeniz önerilir. Kullanıcı düzeyi ayarı, kuruluş düzeyi ayarını geçersiz kılar.

2. Güvenlik varsayılanlarını etkinleştir ayarını Hayır olarak ayarerek Azure **Güvenlik Varsayılanları'nın devre dışı** **bırak:**

    1. Güvenlik yöneticisi, Koşullu Erişim yöneticisi veya genel yönetici olarak Azure portalında oturum açın.
    1. Özellikler'Azure Active Directory >**  gidin** ve Güvenlik **varsayılanlarını yönet'i seçin.**
    1. Güvenlik **varsayılanlarını etkinleştir iki durumlu** ayarını Hayır **olarak ayarlayın.**
    1. **Kaydet**'i seçin.

3. Kullanılan lisanslı posta kutusunda Multi Factor Authentication'ı (MFA) devre dışı bırak.

    1. Gezinti Bölmesi'Microsoft 365 yönetim merkezi ve sol gezinti menüsünde Kullanıcılar Etkin **kullanıcılar'ı**  >  **seçin.**
    1. Etkin kullanıcılar sayfasında **Multi-factor authentication'ı seçin.** 
    1. Kullanıcıyı seçin ve **Multi-Factor Authentication'ı devre dışı bırakın.**

