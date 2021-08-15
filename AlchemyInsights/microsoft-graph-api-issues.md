---
title: Microsoft Graph API sorunları
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
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975913"
---
# <a name="microsoft-graph-api-issues"></a>Microsoft Graph API sorunları

Bu konu, Hala Azure AD Graph API kullanan geliştiriciler için de geçerlidir. Bununla birlikte, **tüm dizin,** kimlik ve erişim yönetimi senaryolarınız Graph Microsoft Graph'i kullanmanız kesinlikle önerilir.

**Kimlik doğrulama veya yetkilendirme sorunları**

- Uygulamanız Microsoft  Graph'i aramak için belirteç alamasa da, bu konuda daha özel yardım ve destek almak için Microsoft Graph erişim belirteci **(Kimlik Doğrulama)** kategorisi alma ile ilgili sorun'u seçin.
- Uygulamanız Microsoft Graph'u arayarak arama sırasında **401 veya 403** yetkilendirme hatası alıyorsa, bu konuda daha özel yardım ve destek almak için Erişim reddedildi hatası **(Yetkilendirme)** Microsoft Graph API'si kategorisini seçin.

**Microsoft Graph'i kullanmak istiyorum ama nereden başlayacağımı bilmiyorum**

- [Microsoft Graph'a genel bakış](https://docs.microsoft.com/graph/overview)
- [Microsoft Graph'ta Kimlik ve Erişim Yönetimi'ne genel Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph uygulamalarını Graph başlarken](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Kiracınız veya tanıtım Graph API'leri test etmek

**Microsoft Graph'i kullanmak istiyorum ama gereken v1.0 dizin API'lerini destekliyor mu?**

Microsoft Graph dizin, kimlik ve erişim yönetimi için önerilen API'dir. Bununla birlikte, Azure AD ad ve Microsoft Graph'da mümkün olan şeyler arasında hala birkaç Graph. Seçiminize yardımcı olacak en güncel farkları vurgulayan aşağıdaki makaleleri gözden geçirin:

- [Azure AD abonelikleri ile Microsoft Graph arasındaki kaynak türü Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD aboneliği ile Microsoft Graph arasındaki özellik Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD ile Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Çağrı yapacağım API çalışmıyor, nereden daha fazla test yapabilirim?**

**Microsoft Graph Explorer** - Kiracı Graph veya tanıtım kiracısı olarak Microsoft Graph API'lerini test edin ve Microsoft Graph Explorer'daki örnek sorgulara göz atabilirsiniz. 

**Uygulamam çok yavaş ve aynı zamanda kısıtlanıyor. Hangi geliştirmeleri ben sağlarim?**

Senaryonıza bağlı olarak, uygulamanın daha iyi performans gösterip uygulamayı daha iyi performans gösterip bazı durumlarda (çok fazla arama yaparken) hizmet tarafından kısıt yapmaya daha az olan çeşitli seçenekler vardır.

- [Microsoft Graph yöntemleri](https://docs.microsoft.com/graph/best-practices-concept)
- [Toplu istekler](https://docs.microsoft.com/graph/json-batching)
- [Değişiklik sorgusu aracılığıyla değişiklikleri izleme](https://docs.microsoft.com/graph/delta-query-overview)
- [Web'ler aracılığıyla değişikliklerle ilgili bilgi al](https://docs.microsoft.com/graph/webhooks)
- [Azaltma kılavuzu](https://docs.microsoft.com/graph/throttling)

**Hatalar ve bilinen sorunlar hakkında daha fazla bilgiyi nereden bulamıyorum?**

- [Microsoft Graph hata yanıtı bilgileri](https://docs.microsoft.com/graph/errors)
- [Microsoft Graph ile ilgili bilinen sorunlar](https://docs.microsoft.com/graph/known-issues)

**Hizmet kullanılabilirliği ve bağlantısının durumunu nereden kontrol olabilirim?**

Microsoft Graph aracılığıyla erişilebilen temel hizmetlerin hizmet kullanılabilirliği ve bağlantısı, Microsoft Graph'nin genel kullanılabilirliğini ve performansını etkileyebilir.

- Hizmet Azure Active Directory durumu için, Azure durum **sayfasında listelenen Güvenlik + Kimlik** hizmetlerinin durumunu kontrol [edin.](https://azure.microsoft.com/status/)
- Microsoft Office bir hizmet Graph daha fazla bilgi için Hizmet Durumu Panosu'Office [listelenen hizmetlerin durumunu kontrol edin.](https://portal.office.com/adminportal/home#/servicehealth)

Microsoft Graph yetkilendirme hataları, çoğu 401 veya 403 hatasına neden olan birkaç farklı hatanın sonucu olabilir. Örneğin, aşağıdakilerin hepsi yetkilendirme hatalarına neden olabilir:

- Yanlış [erişim belirteci edinme akışları](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Kötü yapılandırılmış [izin kapsamları](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- [Onay](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) eksikliği

***Azure Active Directory Authentication Library (ADAL) ve Azure AD Graph API (AAD Graph) için destek sonu***

**30 Haziran 2020'den** itibaren ADAL ve Azure AD Hizmetleri'ne artık yeni bir özellik Graph. Teknik destek ve güvenlik güncellemeleri sağlamaya devam edeceğiz, ancak artık özellik güncellemeleri sunmayacağız.

**30 Haziran 2022'den** itibaren ADAL ve Azure AD Graph artık teknik destek veya güvenlik güncelleştirmeleri sağlamamayacak.

Mevcut işletim sistemi sürümlerinde ADAL kullanan uygulamalar bu sürenin ardından çalışmaya devam edecektir ancak teknik destek *veya güvenlik güncelleştirmelerini almayacaktır.*

Azure AD Graph kullanan uygulamalar bu sürenin ardından artık Azure AD Graph uç Graph almayabilirsiniz.

**ADAL Geçişi**

En son özelliklere ve güvenlik güncellemelerine sahip olan [Microsoft Kimlik Doğrulama Kitaplığı'na (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) güncelleme yapmanızı öneririz.

Microsoft uygulamalarını kullanıyorsanız, Microsoft'un destek bitiş tarihine kadar uygulamalarını MSAL'a en geç geçe kadar MSAL'a bölme sürecinde olduğunu ve MSAL'ın devam eden güvenlik ve özellik geliştirmelerinden yararlanacaklarından, onların da yararlanmasını sağlamayı öğrenin.

1. [ADAL SSS bölümünü okuyunuz](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Uygulamaları platforma göre nasıl taşıyacağınız hakkında bilgi edinin](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Uygulamalardan hangilerinin ADAL'ı kullanabileceğini anlamanız için yardıma ihtiyacınız varsa tüm uygulamalarınızı kaynak kodunu gözden geçirmenizi ve varsa tüm ISVs'lere veya uygulama sağlayıcılarına ulaşmanızı öneririz. Microsoft desteği ayrıca kiracınızdaki Microsoft dışı tüm ADAL uygulamalarının bir listesini de sağlayabilir.

**AAD Graph Geçişi**

Azure AD Graph kullanan uygulamalar için, Azure AD Graph uygulamalarını [Microsoft Graph'e geçirme yönergelerimizi Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Geçiş kontrol listemiz bir başlangıç noktası sağlar.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Azure uygulama kayıt portalınız, hangi uygulamaların AAD Graph kullandığını gösterir. Tüm uygulamalarınızın kaynak kodunu gözden geçirmenizi ve uygunsa, herhangi bir ISV veya uygulama sağlayıcıya ulaşmanızı öneririz. Microsoft desteği, kiracınız için tüm AAD kullanım Graph bir liste de sağlar.
3. Uygulamanın Microsoft Graph'deki verilere erişmesi için, kullanıcının veya yöneticinin izin süreci aracılığıyla bu verilere doğru izinleri olması gerekir. Microsoft [Graph izinleri başvurusu,](https://docs.microsoft.com/graph/permissions-reference) Microsoft kullanıcı api'lerinden her bir ana kümeyle Graph listeler. Ayrıca, izinleri kullanma konusunda yol göstermeyi de sağlar.
