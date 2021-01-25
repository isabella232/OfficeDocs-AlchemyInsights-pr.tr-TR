---
title: Bağlantılar ve URL 'Ler ile ilgili sorunlar
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974757"
---
# <a name="issues-with-links-and-urls"></a>Bağlantılar ve URL 'Ler ile ilgili sorunlar

URI/Reply URL 'Lerini yeniden yönlendir (her iki ifade da her iki ifade da değiştirilebilir), uygulama tarafından istenen belirteçleri döndürmek için Microsoft Identity platform tarafından kullanılan URL 'Ler Bu URL 'Ler hakkında bilgi için aşağıdaki makalelere bakın:

- [Kimlik doğrulama akışları ve uygulama senaryoları](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) -her senaryonun **uygulama kaydı** sayfasında yeniden yönlendirme URI 'leri hakkında bilgi.
- [Yönlendirme URI 'SI/yanıt URL kısıtlamaları ve sınırlamaları](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Uygulamam için RIGHT Redirect URI/Reply URL 'sini nasıl kaydedeceğinizi bilmiyorum**

Geliştirdiğiniz uygulama ile oturum açtığınızda, oturum açma iletişim kutusu **AADSTS50011 görüntülüyorsa: istekte belirtilen yanıt URL 'si uygulama <your app ID> için yapılandırılmış olan yanıt URL 'leriyle eşleşmezse**, uygulama kaydınızı, kod isteğinde kodunuzun Microsoft Identity platformuna KULLANDıĞı yeniden yönlendirme URI 'sini de eklemeniz gerekir.

Bir yanıt URL 'SI eklemek için, Azure portalında **uygulama kayıt** sayfanızda **kimlik doğrulama** sekmesine gidin ve **Uri 'leri yönlendir** bölümüne bir girdi ekleyin. Yönlendirme URI 'Leri yazılır (Web veya mobil/masaüstü). Girmeniz gereken değer, aşağıda açıklandığı gibi, oluşturduğunuz uygulama türüne bağlıdır:

- Tek sayfalık uygulamalar ve Web uygulamaları için, yanıt URL 'SI uygulamanızdaki bir URL olur. Azure portalını kullanarak [tek sayfalı uygulama kaydı](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) veya [Web uygulaması uygulaması kaydettirme](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Masaüstü uygulamaları için, seçmeniz gereken değer aşağıdakilere bağlıdır:
    - Platform (MacOS, Windows veya Linux 'tan farklıdır)
    - Bu belirteci edinme yöntemi (etkileşimli olarak, tümleşik Windows kimlik doğrulaması [ıWA] veya Kullanıcı adı/parola ile).
    Ayrıntılar için bkz: [Masaüstü uygulamaları-App Registration-Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Mobil uygulamalar için, yönlendirme URI 'SI aşağıdakilere bağlıdır:
    - Platform (iOS/Android/UWP)
    - iOS 'daki paket KIMLIĞI ve Android 'deki paket adı ve imza karması gibi uygulamanızı oluşturmak için kullanılan bilgiler, Azure portal uygulaması kaydı size yardımcı olacaktır. Ayrıntılar için [, bkz.](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris)

> [!NOTE]
> Web API 'Leri ve belirteçleri (ıWA ve kullanıcıadı/parola) almanın sessiz yollarından bazıları yeniden yönlendirme URI 'SI gerektirmez.

**Web uygulamamı Kuruluşum ve Dağıtılmış uygulamayı sındığımda, yanıt URL uyumsuzluğu iletisi alıyorum**

Web uygulamanızı dağıttığınız tüm konumlar için yeniden yönlendirme URI 'Leri ekleyin. Daha fazla bilgi için bkz [.](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)

> [!NOTE]
> Uygulamayı bu konumda dağıttıktan hemen sonra bir konum için yeniden yönlendirme URI 'SI ekleyin.

**Yeterli yanıt URL 'Lerini kaydedemiyorum**

Bir ISV kullanıyorsunuz ve size ait her müşteri için bir veya birkaç yeniden yönlendirme Uri 'si vardır. ADAL/Azure AD v 1.0'dan MSAL/Microsoft Identity platformuna geçirmek istiyorsunuz ve [yeniden yönlendirme URI sayısı üst sınırına](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris)ulaşıldı. Bunu çözmek için, müşterilerinize [yönlendirilen URI 'leri hizmet sorumlularına ekleyin](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) .
