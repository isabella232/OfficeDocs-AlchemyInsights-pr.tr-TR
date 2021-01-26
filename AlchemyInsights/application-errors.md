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
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984655"
---
# <a name="application-errors"></a>Uygulama hataları

Azure Active Directory (Azure AD) güvenlik belirteci hizmeti 'nden (STS) döndürülen **Aadsts hata kodları** hakkında bilgi mi arıyorsunuz? ADSTS hata açıklamaları, düzeltmeler ve önerilen bazı geçici çözümler için [Azure AD doğrulama ve yetkilendirme hata kodlarını](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) okuyun.

Yetkilendirme hataları, çoğu ayrı bir 401 veya 403 hatası üreten çeşitli sorunlardan oluşur. Örneğin, aşağıdakiler tüm yetkilendirme hatalarına neden olabilir:

- Yanlış [erişim belirteci alma akışları](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Kötü yapılandırılmış [izin kapsamları](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- [İzin](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) eksikliği

Yaygın kimlik doğrulama hatalarını çözmek için, aşağıdaki adımlardan aldığınız hatayla en yakın şekilde eşleştiğini deneyin. Birden çok bulunabilir.

**401 yetkisiz hatası: belirteciniz geçerli mi?**

Uygulamanızın, isteğin bir parçası olarak Microsoft Graph 'a geçerli bir erişim belirteci sunduğunuzdan emin olun. Bu hata, genellikle erişim belirtecinin HTTP kimlik doğrulaması istek üst bilgisinde eksik olabileceği veya belirtecin geçersiz veya süresinin dolduğu anlamına gelir. Access belirteci alma için [Microsoft kimlik doğrulama kitaplığı 'nı (msal)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) kullanmanızı kesinlikle öneririz. Ayrıca, yalnızca iş veya okul hesaplarını destekleyen bir API 'ye erişmek için kişisel bir Microsoft hesabına atanmış bir temsilci erişim belirtecini kullanmaya çalışırsanız bu hata oluşabilir.

**403 Yasak hatası: doğru izin kümesini seçtiniz misiniz?**

Uygulamanızın çağrı yaptığınız Microsoft Graph API 'Lerine göre doğru izin kümesini istemiş olup olmadığını denetleyin. Önerilen en az ayrıcalıklı izinler tüm Microsoft Graph API başvuru yöntemi konularında sağlanır. Ayrıca, bu izinler bir kullanıcı veya yönetici tarafından uygulamaya verilmelidir. İzinleri normalde izin verme sayfası aracılığıyla veya Azure portal uygulaması kayıt Uygulamanın **Ayarlar** dikey penceresinde, **gerekli izinler**'ı ve sonra **izin ver**'i tıklatın.

- [Microsoft Graph izinleri](https://docs.microsoft.com/graph/permissions-reference) 
- [Azure AD izinlerini ve onayı anlama](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Yasak hatası: uygulamanız seçilen izinleri eşlemek için bir belirteç edindim mu?**

İstenen veya verilen izin türünün, uygulamanızın aldığı erişim belirtecinin türüyle eşleştiğinden emin olun. Uygulama izinlerini isteyebilir ve verebilir, ancak kimlik bilgileri akışı belirteçleri yerine temsilci olarak etkileşimli kod akışı belirteçlerini kullanabilir veya temsilci olarak atanmış izin verme

- [Kullanıcılar adına ve temsilci atama izinlerine erişme](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0-OAuth 2,0 yetkilendirme kodu akışı](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Kullanıcı (daemon hizmeti) ve uygulama izinleri olmadan erişim alma](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v 2.0-OAuth 2,0 istemci kimlik bilgileri akışı](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 Yasak hatası: parola sıfırlanıyor**

Şu anda, kullanıcı parolalarının sıfırlanmasına izin veren uygulama izni Daemon hizmeti hizmeti izinleri yoktur. Bu API 'Ler yalnızca, oturumu açılmış yönetici olan etkileşimli temsilci kod akışları kullanılarak desteklenir.

- [Microsoft Graph izinleri](https://docs.microsoft.com/graph/permissions-reference)

**403 Yasak: kullanıcının erişimi var mı ve lisanslıdır mi?**

Temsilci olarak atanan kod akışları için, uygulamaya verilen izinlere ve oturum açan kullanıcının izinlerine göre isteğe bağlı olarak Microsoft Graph tarafından değerlendirilir. Bu hata genellikle kullanıcının isteği gerçekleştirecek kadar ayrıcalıklı olmadığını veya kullanıcının erişilmekte olduğu veriler için lisanslı olmadığını gösterir. Yalnızca gerekli izinlere veya lisanslara sahip kullanıcılar isteği başarıyla yapabilir.

**403 Yasak: doğru kaynak API 'sini seçmiştiniz mi?**

Microsoft Graph gibi API hizmetleri, alınan erişim belirtecindeki AUD talebinin (hedef kitle) kendisinin gerektirdiği değerle eşleştiğini denetleyin ve değilse, 403 Yasak hatasına neden olur. Bu hatayla sonuçlanan yaygın bir hata, Azure AD grafiği API 'Leri, Outlook API 'leri veya SharePoint/OneDrive API 'Lerinin Microsoft Graph (veya tam tersi) için edinildiği bir belirteç kullanmaya çalışıyor. Uygulamanızın çağrı yaptığınız API ile eşleşen bir belirteç aldığından emin olun.

**400 Hatalı Istek veya 403 Yasak: Kullanıcı, kuruluşlarının koşullu erişim (CA) ilkelerine uygun mu?**

Bir kuruluşun CA ilkelerine bağlı olarak, uygulamanız aracılığıyla Microsoft Graph kaynaklarına erişen bir Kullanıcı, uygulamanızın ilk edinildiği erişim belirtecinde bulunmayan ek bilgiler için sizi umsunmayabilir. Bu durumda, uygulamanız Access belirteci alımı veya Microsoft Graph 'ı ararken *insufficient_claims* hatasını içeren 403 *interaction_required* hatasıyla bir 400 alır. Her iki durumda da, hata yanıtı, kullanıcının ek bilgi (Multi-Factor Authentication veya Device kaydı gibi) için kimlik doğrulama uç noktasına sunulabilecek ek bilgiler içerir.

- [MSAL kullanarak koşullu erişim sorunlarını işleme ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Azure Active Directory Koşullu erişimi için Geliştirici Kılavuzu](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
