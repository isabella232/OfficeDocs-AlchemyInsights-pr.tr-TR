---
title: Uygulama hataları
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931469"
---
# <a name="application-errors"></a>Uygulama hataları

AZURE ACTIVE DIRECTORY (Azure AD) güvenlik belirteci hizmetlerinden (STS) döndürülen **AADSTS** hata kodları hakkında bilgi mi arıyorsunuz? AADSTS [hata açıklamalarını,](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) düzeltmelerini ve önerilen bazı geçici çözümleri bulmak için Azure AD Kimlik Doğrulama ve yetkilendirme hata kodlarını okuyun.

Yetkilendirme hataları, çoğu 401 veya 403 hatası oluşturan birkaç farklı sorunun sonucu olabilir. Örneğin, aşağıdakilerin hepsi yetkilendirme hatalarına neden olabilir:

- Yanlış [erişim belirteci edinme akışları](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Kötü yapılandırılmış [izin kapsamları](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- [Onay](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) eksikliği

Yaygın yetkilendirme hatalarını çözmek için, aşağıda verilen ve alırsınız hataya en yakın şekilde eşleşen adımları deneyin. Birden fazla başvuru olabilir.

**401 Yetkisiz hata: Belirteciniz geçerli mi?**

İsteğin bir parçası olarak, uygulamanın Microsoft Graph bir erişim belirteci sun olduğundan emin olun. Bu hata genellikle erişim belirtecinin HTTP kimlik doğrulama isteği başlığında eksik olabileceği veya belirtecin geçersiz veya süresi dolmuş olabileceği anlamına gelir. Erişim belirteci alımı için [Microsoft Kimlik Doğrulama Kitaplığı'nın (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) kullanımını kesinlikle öneririz. Buna ek olarak, yalnızca iş veya okul hesaplarını (kuruluş hesapları) destekleyen bir API'ye erişmek için kişisel Microsoft hesabına verilen temsili erişim belirteci kullanmaya çalışırsanız bu hata oluşabilir.

**403 Yasak hata: Doğru izin kümesini seçtiniz mi?**

Uygulama aramalarınızı alan Microsoft Veri Api'lerine dayalı olarak doğru izin Graph isteğinizi denetleyin. Tüm Microsoft Graph API başvuru yöntemi konularında önerilen en Graph izinler sağlanır. Ek olarak, bu izinlerin uygulamaya bir kullanıcı veya yönetici tarafından verilmesi gerekir. İzinlerin verilmesi normalde bir izin sayfası üzerinden veya Azure Portal uygulama kayıt blade'i kullanılarak izin verilmesiyle gerçekleşir. Uygulamanın **Ayarlar** penceresinden, **Gerekli İzinler** öğesine tıklayın ve ardından **İzinleri Ver** öğesine tıklayın.

- [Microsoft Graph izinleri](https://docs.microsoft.com/graph/permissions-reference) 
- [Azure AD izinlerini ve onayını anlama](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Yasak hata: Uygulamanız seçilen izinlerle eşleşecek bir jeton aldı mı?**

İstenen veya verilen izinlerin türünün, uygulamanız tarafından alınan erişim belirteci türüyle aynı olduğundan emin olun. Uygulama izinleri ister ve vermekle birlikte, istemci kimlik bilgisi akış belirteçleri yerine temsili etkileşimli kod akış belirteçleri kullanıyor veya temsili izinler talep ediyor ve vermekle birlikte, temsili kod akış belirteçleri yerine istemci kimlik bilgisi akış belirteçleri kullanıyor da olabilirsiniz.

- [Kullanıcılar ve yetki verilen izinler adına erişim elde edin](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - OAuth 2.0 yetkilendirme kodu akışı](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Kullanıcı (arka plan programı hizmeti) ve uygulama izinleri olmadan erişim sağlayın](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - OAuth 2.0 istemci kimlik bilgileri akışı](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 Yasak hata: Parola sıfırlamak**

Şu anda, kullanıcı parolalarının sıfırlanmasına izin veren arka plan programı hizmetinden hizmete yönelik uygulama izni yoktur. Bu API'ler, yalnızca oturum açmış bir yönetici ile etkileşimli, yetki verilmiş kod akışları kullanılarak desteklenir.

- [Microsoft Graph izinleri](https://docs.microsoft.com/graph/permissions-reference)

**403 Yasak: Kullanıcının erişimi var mı ve lisanslı mı?**

Temsili kod akışları için Microsoft Graph, uygulamaya verilen izinlere ve oturum açmış kullanıcının sahip olduğu izinlere bağlı olarak, isteğin izin veriip verilme verilmeyecektir. Genel olarak bu hata, kullanıcının isteği gerçekleştirecek kadar ayrıcalıklı olmadığını veya kullanıcının erişilen veriler için lisansının olmadığını gösterir. Yalnızca gerekli izinlere veya lisanslara sahip kullanıcılar istekte başarılı olabilir.

**403 Yasak: Doğru kaynak API'sini seçtiniz mi?**

Microsoft Graph API hizmetleri, alınan erişim belirteci'nde yer alan aud talebinin (hedef kitlenin) kendisi için beklenilen değerle eşlenip eşleşme olmadığını kontrol eder ve eşleşmezse 403 Yasak hatasıyla sonuç verir. Bu hatayla sonuçlanan yaygın bir hata, Azure AD Graph API'leri, Outlook API'leri veya SharePoint/OneDrive API'leri için alınan bir belirteci Microsoft Graph'ı çağırmak için kullanmaya çalışmaktır (veya tam tersi). Uygulamanızın, uygulamanın çağırdığı API ile eşleşmek üzere bir belirteç elde ettiğinden emin olun.

**400 Hatalı İstek veya 403 Yasak: Kullanıcı, kuruluşun koşullu erişim (CA) politikalarına uyuyor mu?**

Kuruluşun CA ilkelerine bağlı olarak, Microsoft Graph kaynaklarına kendi uygulamanız üzerinden erişen bir kullanıcı, başlangıçta edinilen erişim belirtecsinde yer alan ek bilgiler için zor olabilir. Bu durumda, uygulamanız erişim belirteci edinme sırasında bir *etkileşim_gerekli* hata içeren bir 400 veya Microsoft Graph arandığında *yetersiz_talep hatası içeren bir* 403 alır. Her iki durumda da, hata yanıtı ek bilgi için (çok faktörlü kimlik doğrulaması veya cihaz kaydı gibi) kullanıcıya meydan okumak için yetki uç noktasına sunabilirsiniz ek bilgiler içerir.

- [MSAL kullanarak koşullu erişim güçlüklerini işleme ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Azure Active Directory koşullu erişimi için geliştirici kılavuzu](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
