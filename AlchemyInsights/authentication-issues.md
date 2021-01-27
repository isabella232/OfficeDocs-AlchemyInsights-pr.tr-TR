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
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976869"
---
# <a name="authentication-issues"></a>Kimlik doğrulama sorunları

**Azure Active Directory (Azure AD) güvenlik belirteci hizmetinden (STS) döndürülen AADSTS hata kodları hakkında bilgi mi arıyorsunuz?** AADSTS hata açıklamalarını, düzeltmeleri ve önerilen bazı geçici çözümleri bulmak için [Azure AD Kimlik Doğrulaması ve yetkilendirme hata kodlarını](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) inceleyin.

Yetkilendirme hataları, çoğu 401 veya 403 hatası oluşturan birkaç farklı sorunun sonucu olabilir. Örneğin, aşağıdaki sorunların tümü yetkilendirme hatalarına yol açabilir:

- Yanlış [erişim belirteci edinme akışları](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Kötü yapılandırılmış [izin kapsamları](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- [Onay](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent) eksikliği

Yaygın yetkilendirme hatalarını çözmek için, aldığınız hatayla en yakından eşleşen, aşağıda verilen adımları deneyin. Aldığınız bir hata için birden fazla adım geçerli olabilir.

**401 Yetkisiz hata: Belirteciniz geçerli mi?**

Uygulamanızın, isteğin bir parçası olarak Microsoft Graph'a geçerli bir erişim belirteci sunduğundan emin olun. Bu hata genellikle erişim belirtecinin HTTP kimlik doğrulama isteği başlığında eksik olabileceği veya belirtecin geçersiz veya süresi dolmuş olabileceği anlamına gelir. Erişim belirteci edinimi için Microsoft Kimlik Doğrulama Kitaplığı'nı (MSAL) kullanmanızı şiddetle tavsiye ederiz. Ayrıca, yalnızca iş veya okul hesaplarını (kurumsal hesaplar) destekleyen bir API'ye erişmek için kişisel bir Microsoft hesabına verilen temsilci erişim belirtecini kullanmaya çalışırsanız bu hata oluşabilir.

**403 Yasak hata: Doğru izin kümesini seçtiniz mi?**

Uygulamanızın çağırdığı Microsoft Graph API'lerine göre doğru izin kümesini talep ettiğinizden emin olun. Önerilen en az ayrıcalıklı izinler, tüm Microsoft Graph API başvuru yöntemi konularında sağlanmaktadır. Ek olarak, bu izinlerin uygulamaya bir kullanıcı veya yönetici tarafından verilmesi gerekir. İzinlerin verilmesi normalde bir izin sayfası veya Azure Portal uygulama kayıt penceresi kullanılarak gerçekleşir. Uygulamanın **Ayarlar** penceresinden, **Gerekli İzinler** öğesine tıklayın ve ardından **İzinleri Ver** öğesine tıklayın. Daha fazla bilgi için bkz.:

- [Microsoft Graph izinleri](https://docs.microsoft.com/graph/permissions-reference) 
- [Azure AD izinlerini ve onayını anlama](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Yasak hata: Uygulamanız seçilen izinlerle eşleşecek bir jeton aldı mı?**

İstenen veya verilen izin türlerinin, uygulamanızın aldığı erişim belirteci türüyle eşleştiğinden emin olun. Uygulama izinleri istiyor ve veriyor olabilirsiniz, ancak istemci kimlik bilgisi akış belirteçleri yerine temsilci olarak atanmış etkileşimli kod akış belirteçleri kullanıyor olabilirsiniz, veya temsilci atanmış izinler isteme ve verme, temsilci kod akış belirteçleri yerine istemci kimlik bilgisi akış belirteçleri kullanma.

Belirteç edinmeyle ilgili daha fazla bilgi için, bakınız:

- [Kullanıcılar ve yetki verilen izinler adına erişim elde edin](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 - OAuth 2.0 yetkilendirme kodu akışı](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Kullanıcı (arka plan programı hizmeti) ve uygulama izinleri olmadan erişim sağlayın](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 - OAuth 2.0 istemci kimlik bilgileri akışı](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 Yasak hata: Parola sıfırlamak**

Şu anda, kullanıcı parolalarının sıfırlanmasına izin veren arka plan programı hizmetinden hizmete yönelik uygulama izni yoktur. Bu API'ler, yalnızca oturum açmış bir yönetici ile etkileşimli, yetki verilmiş kod akışları kullanılarak desteklenir. Daha fazla bilgi için bkz. [Microsoft Graph izinleri](https://docs.microsoft.com/graph/permissions-reference).

**403 Yasak: Kullanıcının erişimi var mı ve lisanslı mı?**

Temsilci olarak atanan kod akışları için Microsoft Graph, uygulamaya verilen izinlere ve oturum açmış kullanıcının sahip olduğu izinlere göre isteğe izin verilip verilmediğini değerlendirir. Genel olarak bu hata, kullanıcının isteği gerçekleştirecek kadar ayrıcalıklı olmadığını **veya** kullanıcının erişilen veriler için lisansının olmadığını gösterir. Yalnızca gerekli izinlere veya lisanslara sahip kullanıcılar istekte başarılı olabilir.

**403 Yasak: Doğru kaynak API'sini seçtiniz mi?**

Microsoft Graph gibi API hizmetleri, alınan erişim belirtecindeki *aud* talebinin (hedef kitle) kendisi için beklediği değerle eşleşip eşleşmediğini kontrol eder ve aksi takdirde 403 Yasak hatası oluşur. Bu hatayla sonuçlanan yaygın bir hata, Azure AD Graph API'leri, Outlook API'leri veya SharePoint/OneDrive API'leri için alınan bir belirteci Microsoft Graph'ı çağırmak için kullanmaya çalışmaktır (veya tam tersi). Uygulamanızın, uygulamanın çağırdığı API ile eşleşmek üzere bir belirteç elde ettiğinden emin olun.

**400 Hatalı İstek veya 403 Yasak: Kullanıcı, kuruluşun koşullu erişim (CA) politikalarına uyuyor mu?**

Bir kuruluşun koşullu erişim (CA) politikalarına göre, uygulamanız aracılığıyla Microsoft Graph kaynaklarına erişen bir kullanıcı, uygulamanızın ilk olarak edindiği erişim belirtecinde bulunmayan ek bilgiler için sorgulanabilir. Bu durumda, **uygulamanız erişim belirteci edinme sırasında bir *etkileşim_gerekli* hata içeren bir** 400 veya **Microsoft Graph arandığında *yetersiz_talep* hatası içeren bir** 403 alır. Her iki durumda da, hata yanıtı, kullanıcıyı ek bilgi için sorgulamak üzere yetkili uç noktaya sunulabilecek ek bilgileri içerir (çok faktörlü kimlik doğrulama veya cihaz kaydı gibi).

Koşullu erişimle ilgili daha fazla bilgi için bkz :

- [MSAL kullanarak koşullu erişim zorluklarının üstesinden gelme](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Azure Active Directory koşullu erişimi için geliştirici kılavuzu](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Azure Active Directory Authentication Library (ADAL) ve Azure AD Graph API (AAD Graph) desteğinin sonu_* _

- 30 Haziran 2020'den itibaren Azure Active Directory Authentication Library (ADAL) ve Azure AD Graph API'ye (AAD Graph) artık yeni özellikler eklemeyeceğiz. Teknik destek ve güvenlik güncellemeleri sağlamaya devam edeceğiz, ancak artık özellik güncellemeleri sunmayacağız.
- 30 Haziran 2022'den itibaren, ADAL ve AAD Grafiği için desteği sona erdireceğiz ve artık teknik destek veya güvenlik güncellemeleri sunmayacağız.
    - Mevcut işletim sistemi sürümlerinde ADAL kullanan uygulamalar bu süreden sonra çalışmaya devam edecek ancak herhangi bir teknik destek veya güvenlik güncellemesi almayacaktır.
    - Bu süreden sonra AAD Graph kullanan uygulamalar artık AAD Graph uç noktasından yanıt alamayabilir.

_ *ADAL Geçişi**

En son özelliklere ve güvenlik güncellemelerine sahip olan [Microsoft Kimlik Doğrulama Kitaplığı'na (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) güncelleme yapmanızı öneririz. Bu öneri, Microsoft'un uygulamalarını destek sonu son tarihine kadar MSAL'a geçirmesi bağlamındadır. Microsoft uygulamalarının MSAL'a geçişinin amacı, uygulamaların MSAL'ın devam eden güvenlik ve özellik iyileştirmelerinden yararlanmasını sağlamaktır.

- [ADAL SSS bölümünü okuyunuz](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Uygulamaları platforma göre nasıl taşıyacağınız hakkında bilgi edinin](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Hangi uygulamalarınızın ADAL kullandığını anlamak için yardıma ihtiyacınız varsa, tüm uygulamalarınızın kaynak kodunu gözden geçirmenizi ve uygunsa, herhangi bir bağımsız yazılım satıcısına (ISV) veya uygulama sağlayıcıya ulaşmanızı öneririz. Microsoft desteği ayrıca kiracınızdaki Microsoft dışı tüm ADAL uygulamalarının bir listesini de sağlayabilir.

**AAD Graph Geçişi**

AAD Graph kullanan uygulamalar için [Azure AD Graph uygulamalarını Microsoft Graph'a geçirmek](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true) için rehberimizi izleyin.

- [Geçiş kontrol listemiz bir başlangıç noktası sağlar.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
- Azure uygulama kayıt portalınız, hangi uygulamaların AAD Graph kullandığını gösterir. Tüm uygulamalarınızın kaynak kodunu gözden geçirmenizi ve uygunsa, herhangi bir ISV veya uygulama sağlayıcıya ulaşmanızı öneririz. Microsoft Desteği ayrıca size kiracınızdaki tüm AAD Graph kullanımı hakkında bilgi sağlayabilir.

 










