---
title: Kimlik doğrulama sorunları
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974788"
---
# <a name="authentication-issues"></a>Kimlik doğrulama sorunları

**Azure Active Directory (Azure AD) güvenlik belirteci hizmeti 'nden (STS) döndürülen AADSTS hata kodları hakkında bilgi mi arıyorsunuz?** ADSTS hata açıklamaları, düzeltmeler ve önerilen bazı geçici çözümler için [Azure AD doğrulama ve yetkilendirme hata kodlarına](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) bakın.

Yetkilendirme hataları, çoğu ayrı bir 401 veya 403 hatası üreten çeşitli sorunlardan oluşur. Örneğin, aşağıdaki sorunlar tüm yetkilendirme hatalarına neden olabilir:

- Yanlış [erişim belirteci alma akışları](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Kötü yapılandırılmış [izin kapsamları](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- [İzin](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent) eksikliği

Yaygın kimlik doğrulama hatalarını çözmek için, aldığınız hatayla en yakın şekilde eşleşen aşağıdaki adımları deneyin. Aldığınız bir hata için birden fazla adım uygulanabilir.

- **401 yetkisiz hatası: belirteciniz geçerli mi?**

Uygulamanızın, isteğin bir parçası olarak Microsoft Graph 'a geçerli bir erişim belirteci sunduğunuzdan emin olun. Bu hata, genellikle erişim belirtecinin HTTP kimlik doğrulaması istek üst bilgisinde eksik olabileceği veya belirtecin geçersiz veya süresinin dolduğu anlamına gelir. Access belirteci alma için Microsoft kimlik doğrulama kitaplığı 'nı (MSAL) kullanmanızı kesinlikle öneririz. Ayrıca, yalnızca iş veya okul hesaplarını destekleyen bir API 'ye erişmek için kişisel bir Microsoft hesabına atanmış bir temsilci erişim belirtecini kullanmaya çalışırsanız bu hata ortaya çıkabilir.

**403 Yasak hatası: doğru izin kümesini seçtiniz misiniz?**

Uygulamanızın çağrı yaptığınız Microsoft Graph API 'Lerine göre doğru izin kümesini istemiş olduğunuzdan emin olun. Önerilen en az ayrıcalıklı izinler tüm Microsoft Graph API başvuru yöntemi konularında sağlanır. Ayrıca, bu izinler bir kullanıcı veya yönetici tarafından uygulamaya verilmelidir. İzinleri normal olarak verme, bir izin sayfası veya Azure portal uygulaması kayıt Blade kullanımı aracılığıyla gerçekleşir. Uygulamanın **Ayarlar** dikey penceresinde, **gerekli izinler**'ı ve sonra **izin ver**'i tıklatın. Daha fazla bilgi için bkz.:

- [Microsoft Graph izinleri](https://docs.microsoft.com/graph/permissions-reference) 
- [Azure AD izinlerini ve onayı anlama](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Yasak hatası: uygulamanız seçilen izinleri eşlemek için bir belirteç edindim mu?**

İstenen veya verilen izin türlerinin, uygulamanızın aldığı erişim belirtecinin türüyle eşleştiğinden emin olun. Uygulama izinleri isteyebilir, ancak istemci kimlik bilgileri akış belirteçleri yerine temsilci olarak etkileşimli kod akışı belirteçlerini kullanarak ya da temsilci izni isteyerek veya temsilci olarak atanan kod akışı belirteçleri yerine istemci kimlik bilgileri akış belirteçlerini kullanarak, uygulama izinleri isteyebilir.

Belirteçleri alma hakkında daha fazla bilgi için bkz:

- [Kullanıcılar adına ve temsilci atama izinlerine erişme](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0-OAuth 2,0 yetkilendirme kodu akışı](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Kullanıcı (daemon hizmeti) ve uygulama izinleri olmadan erişim alma](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v 2.0-OAuth 2,0 istemci kimlik bilgileri akışı](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 Yasak hatası: parola sıfırlanıyor**

Şu anda, kullanıcı parolalarının sıfırlanmasına izin veren uygulama izni Daemon hizmeti hizmeti izinleri yoktur. Bu API 'Ler yalnızca, oturumu açılmış yönetici olan etkileşimli temsilci kod akışları kullanılarak desteklenir. Daha fazla bilgi [için bkz.](https://docs.microsoft.com/graph/permissions-reference)

**403 Yasak: kullanıcının erişimi var mı ve lisanslıdır mi?**

Temsilci seçilen kod akışları için, Microsoft Graph, uygulamaya verilen izinlere ve oturum açan kullanıcının izinlerine göre istekte bulunup bulunmayacağını hesaplar. Bu hata genellikle kullanıcının isteği gerçekleştirecek kadar ayrıcalıklı olmadığını **veya** kullanıcının erişilmekte olduğu veriler için lisanslı olmadığını gösterir. Yalnızca gerekli izinlere veya lisanslara sahip kullanıcılar isteği başarıyla yapabilir.

**403 Yasak: doğru kaynak API 'sini seçmiştiniz mi?**

Microsoft Graph gibi API hizmetleri, alınan erişim belirtecindeki *AUD* talebinin (hedef kitle) kendisinin gerektirdiği değerle eşleştiğini denetleyin ve değilse, 403 Yasak hatası oluşur. Bu hatayla sonuçlanan yaygın bir hata, Azure AD grafiği API 'Leri, Outlook API 'leri veya SharePoint/OneDrive API 'Lerinin Microsoft Graph (veya tam tersi) için edinildiği bir belirteç kullanmaya çalışıyor. Uygulamanızın çağrı yaptığınız API ile eşleşen bir belirteç aldığından emin olun.

**400 Hatalı Istek veya 403 Yasak: Kullanıcı, kuruluşlarının koşullu erişim (CA) ilkelerine uygun mu?**

Bir kuruluşun koşullu erişim (CA) ilkelerine bağlı olarak, uygulamanız aracılığıyla Microsoft Graph kaynaklarına erişen bir Kullanıcı, uygulamanızın ilk edinildiği erişim belirtecinde bulunmayan ek bilgiler için sizi umsunmayabilir. Bu durumda, uygulamanız Access belirteci alımı veya Microsoft Graph 'ı ararken ***insufficient_claims* hatasını içeren 403** ***interaction_required*** hatasıyla bir 400 alır. Her iki durumda da, hata yanıtı, kullanıcının ek bilgi (Multi-Factor Authentication veya Device kaydı gibi) için, yetkili uç noktasına sunulabilecek ek bilgiler içerir.

Koşullu erişimle ilgili daha fazla bilgi için bkz:

- [MSAL kullanarak koşullu erişim sorunlarını işleme](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Azure Active Directory Koşullu erişimi için Geliştirici Kılavuzu](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Azure Active Directory kimlik doğrulama kütüphanesi (ADAL) ve Azure AD GRAFIĞI API (AAD Graph) _ desteği sonu_*

- 30 Haziran 2020 ' de başlıyor, artık Azure Active Directory kimlik doğrulama kitaplığı (ADAL) ve Azure AD grafiği API (AAD Graph) için yeni özellikler ekleyemeyecektir. Teknik destek ve güvenlik güncelleştirmelerini sağlamaya devam edeceğiz ancak artık özellik güncelleştirmeleri sağlamaz.
- 30 Haziran 2022 ' de başlıyor, ADAL ve AAD Graph için desteği sona eririz ve artık teknik destek veya güvenlik güncelleştirmeleri sağlamaz.
    - Mevcut işletim sistemi sürümlerinde ADAL kullanan uygulamalar, bu saatten sonra çalışmaya devam edecektir, ancak teknik destek veya güvenlik güncelleştirmelerini alamaz.
    - Bu saatten sonra AAD grafiği kullanan uygulamalar artık AAD grafik uç noktasından yanıt alamaz.

_ *Adal geçişi**

En son özellikleri ve güvenlik güncelleştirmelerini içeren [Microsoft kimlik doğrulama kitaplığı (msal)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)güncelleştirmesini öneririz. Bu öneri, Microsoft 'un uygulamalarını bu süre sonu son tarihine kadar MSAL. Microsoft uygulamalarının MSAL 'e geçişin amacı, uygulamaların MSAL 'un devam eden güvenlik ve özellik geliştirmelerinin avantajlarından yararlanmasını sağlar.

- [ADAL SSS 'sini okuyun](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Uygulamaları platforma göre nasıl geçirebileceğiniz hakkında bilgi edinin](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Hangi uygulamalarınızı ADAL kullanarak anladığınızdan yardım gerekirse, tüm uygulamalarınızın kaynak kodunu gözden geçirmenizi ve varsa tüm bağımsız yazılım satıcılarına (ISV 'Ler) veya uygulama sağlayıcılarını gözden geçirmenizi öneririz. Microsoft desteği size kiracınızdaki Microsoft olmayan tüm ADAL uygulamalarının bir listesini sağlayabilir.

**AAD grafik geçişi**

AAD grafiğini kullanan uygulamalar için, [Azure AD grafiği uygulamalarını Microsoft Graph 'a geçirmek](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true)için kılavuzumuzu izleyin.

- [Geçiş denetim listesi başlangıç noktası sağlar](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Azure App Registration Portal 'da, AAD grafiğini kullanan uygulamalar gösterilir. Tüm uygulamalarınızın kaynak kodunu incelemenizi öneririz ve uygulanabiliyorsa, herhangi bir ISV veya uygulama sağlayıcısına ulaşın. Microsoft destek, kiracınızdaki tüm AAD grafik kullanımının bilgilerini de sağlayabilir.

 










