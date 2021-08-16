---
title: Bağlantılar ve URL'lerle ilgili sorunlar
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 1387d7e0cdf2e730b2812f3970181d2bf889d44b1faab9a351911840909defb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054818"
---
# <a name="issues-with-links-and-urls"></a>Bağlantılar ve URL'lerle ilgili sorunlar

Yönlendirme URI'si/yanıt URL'leri (her iki ifade de birbirinin yerine kullanılabilir) uygulamanın istediği belirteçleri geri döndürmek için Microsoft kimlik platformu tarafından kullanılan URL'lerdir. Bu URL'ler hakkında bilgi için aşağıdaki makalelere bakabilirsiniz:

- [Kimlik doğrulama akışları ve uygulama senaryoları](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Her senaryo için **Uygulama kaydı** sayfasındaki yönlendirme URI'leri hakkında bilgiler.
- [Yönlendirme URI'si/yanıt URL'leri kısıtlamaları ve sınırlamaları](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Uygulamam için doğru yönlendirme URI'si / yanıt URL'lerini nasıl kaydedeceğimi bilmiyorum**

Geliştirdiğiniz uygulamayla oturum açtığınızda oturum açma iletişim kutusu **AADSTS50011 gösteriyorsa: İstekte belirtilen yanıt URL'si, <your app ID>** adlı uygulamanız için yapılandırılmış URL'ler ile eşleşmiyor. Microsoft kimlik platformuna belirteç isteğinde kullanılan kodunuzun yeniden yönlendirme URI'sini uygulama kaydınıza eklemeniz gerekir.

Yanıt URL'si eklemek için, Azure portalda bulunan **uygulama kayıt** sayfasındaki **Kimlik Doğrulaması** sekmesine gidin ve **Yönlendirme URI'leri** bölümüne bir girdi ekleyin. Girmeniz gereken değer, aşağıda açıklandığı gibi oluşturduğunuz uygulama türüne bağlıdır:

- Tek sayfalı uygulamalar ve web uygulamaları için yanıt URL'si uygulamanızdaki bir URL'dir. Bkz: [Tek sayfalı uygulama kaydı](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) veya [Azure portal kullanarak bir web uygulamasını kaydetme](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Masaüstü uygulamalarınız için seçmeniz gereken değer şunlara bağlıdır:
    - platform (MacOS, Windows veya Linux'ten farklıdır)
    - belirteci edinme yönteminiz (etkileşimli olarak, cihaz kodu akışıyla, Tümleşik Windows Kimlik Doğrulaması [IWA] ile veya kullanıcı adı/parolayla).
    Ayrıntılar için bkz: [Masaüstü uygulamaları - Uygulama kaydı - Yönlendirme URI'si](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Mobil uygulamalar için yönlendirme URI'si şunlara bağlıdır:
    - platform (iOS/Android/UWP)
    - iOS'taki paket kimliği, Android'deki paket adı ve imza karması gibi uygulamanızı oluşturmak için kullanılan bilgiler. Azure portal uygulaması kaydı size yardımcı olacaktır. Ayrıntılar için bkz: [Platform yapılandırması ve yönlendirme URI'leri](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Web API'leri ve belirteç almanın bazı sessiz yolları (IWA ve kullanıcı adı/parola) yönlendirme URI'si gerektirmez.

**Web uygulamamı dağıttım ve dağıtılan uygulamayı test ettiğimde, yanıt URL'sinin uymadığına yönelik mesaj alıyorum.**

Web uygulamanızı dağıttığınız tüm konumlar için yönlendirme URI'leri ekleyin. Daha fazla bilgi için bkz: [Azure portal kullanarak bir web uygulamasını kaydetme](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Uygulamayı o konumda dağıttıktan hemen sonra yönlendirme URI'sini konum için ekleyin.

**Yeterli yanıt URL'si kaydedemiyorum**

Her müşteriniz için bir veya birkaç yönlendirme URI'sinizin olduğu bir bağımsız yazılım satıcısısınız. ADAL/Azure Active Directory v1.0'dan MSAL/Microsoft kimlik platformuna geçirmek istiyorsunuz ve [en fazla yönlendirme URI'si sayısına ulaştınız](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Bunu çözmek için her bir müşterinize karşılık gelen [hizmet ilkelerine yeniden yönlendirme URI'leri ekleyin.](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals)
