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
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714517"
---
# <a name="microsoft-graph-api-issues"></a>Microsoft Graph API sorunları

Bu konu, hala Azure AD Graph API kullanan geliştiriciler için de geçerli olabilir. Bununla birlikte, **tüm dizin,** kimlik ve erişim yönetimi senaryolarınız için Microsoft Graph'i kullanmanız kesinlikle önerilir.

**Kimlik doğrulama veya yetkilendirme sorunları**

- Uygulamanız Microsoft Graph **çağrısı** yapmak için belirteç alamasa da, bu konuda daha özel yardım ve destek almak için erişim belirteci **(Kimlik Doğrulama)** Microsoft Graph kategorisi alma ile ilgili Sorun'u seçin.
- Uygulamanız Microsoft Graph'i arama sırasında **401 veya 403** yetkilendirme hatası alıyorsa, bu konuda daha özel yardım ve destek almak için Erişim reddedildi hatası **(Yetkilendirme)** Microsoft Graph API kategorisini seçin.

**Microsoft Graph'i kullanmak istiyorum, ancak nereden başlayacağımdan emin değilim**

- [Microsoft Graph'a genel bakış](https://docs.microsoft.com/graph/overview)
- [Microsoft Graph'te Kimlik ve Erişim Yönetimine Genel Bakış](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph uygulamaları yapmaya başlama](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Kiracı veya tanıtım kiracısı içinde Microsoft Graph API'lerini test

**Microsoft Graph'i kullanmak istiyorum, ancak ihtiyacım olan v1.0 dizin API'lerini destekliyor mu?**

Microsoft Graph dizin, kimlik ve erişim yönetimi için önerilen API'dir. Bununla birlikte, Azure AD Graph ve Microsoft Graph'te mümkün olan şeyler arasında hala birkaç boşluk vardır. Seçiminize yardımcı olmak için en güncel farkları vurgulayan aşağıdaki makaleleri gözden geçirin:

- [Azure AD Graph ile Microsoft Graph arasındaki kaynak türü farklılıkları](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graph ile Microsoft Graph arasındaki özellik farklılıkları](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD ile Microsoft Graph arasındaki yöntem farklılıkları](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Çağrı yapacağım API çalışmıyor, daha fazla test nereden yapabilirim?**

**Microsoft Graph Explorer** - Kiracınız veya tanıtım kiracısı olan Microsoft Graph API'lerini test edin ve Microsoft Graph Explorer'daki **örnek** sorgulara göz atabilirsiniz.

**Uygulamam çok yavaş ve aynı zamanda kısıtlanıyor. Hangi geliştirmeleri ben yapmak için?**

Senaryona bağlı olarak, uygulamanızı daha iyi performans ortaya çıkarmanızı ve bazı durumlarda da hizmet tarafından azaltmaya (çok fazla arama yaparken) daha az açık hale gelen çeşitli seçenekler vardır.

- [Microsoft Graph en iyi yöntemleri](https://docs.microsoft.com/graph/best-practices-concept)
- [Toplu istekler](https://docs.microsoft.com/graph/json-batching)
- [Değişiklik sorgusu aracılığıyla değişiklikleri izleme](https://docs.microsoft.com/graph/delta-query-overview)
- [Web'ler aracılığıyla değişikliklerle ilgili bilgi al](https://docs.microsoft.com/graph/webhooks)
- [Azaltma kılavuzu](https://docs.microsoft.com/graph/throttling)

**Hatalar ve bilinen sorunlar hakkında nereden daha fazla bilgi bulamıyorum?**

- [Microsoft Graph hata yanıt bilgileri](https://docs.microsoft.com/graph/errors)
- [Microsoft Graph ile ilgili bilinen sorunlar](https://docs.microsoft.com/graph/known-issues)

**Hizmet kullanılabilirliği ve bağlantısının durumunu nereden kontrol edeceğim?**

Microsoft Graph aracılığıyla erişilebilen temel hizmetlerin hizmet kullanılabilirliği ve bağlantısı, Microsoft Graph'in genel kullanılabilirliğini ve performansını etkileyebilir.

- Azure Active Directory hizmetinin durumu için, Azure durum sayfasında listelenen **Güvenlik + Kimlik** hizmetlerinin durumunu kontrol [edin.](https://azure.microsoft.com/status/)
- Microsoft Graph'e katkıda bulunan Office hizmetleri için, Office Hizmet Durumu Panosunda listelenen [hizmetlerin durumunu kontrol edin.](https://portal.office.com/adminportal/home#/servicehealth)

Microsoft Graph yetkilendirme hataları, çoğu 401 veya 403 hatası oluşturan çeşitli sorunların sonucu olabilir. Örneğin, aşağıdakilerin hepsi yetkilendirme hatalarına neden olabilir:

- Yanlış [erişim belirteci edinme akışları](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Kötü yapılandırılmış [izin kapsamları](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- [Onay](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) eksikliği

**_Azure Active Directory Authentication Library (ADAL) ve Azure AD Graph API (AAD Graph) desteğinin sonu_* _

_*30 Haziran 2020'den itibaren** artık ADAL ve Azure AD Graph'e yeni özellikler eklemeyecek. Teknik destek ve güvenlik güncellemeleri sağlamaya devam edeceğiz, ancak artık özellik güncellemeleri sunmayacağız.

**30 Haziran 2022'den** başlayarak, ADAL ve Azure AD Graph desteğini sona erecek ve artık teknik destek veya güvenlik güncelleştirmeleri sağmayacak.

Mevcut işletim sistemi sürümlerinde ADAL kullanan uygulamalar bu sürenin ardından çalışmaya devam edecektir, ancak teknik destek *veya güvenlik güncelleştirmelerini almayacaktır.*

Bu sürenin ardından Azure AD Graph kullanan uygulamalar artık Azure AD Graph uç noktasının yanıtlarını almayabilirsiniz.

**ADAL Geçişi**

En son özelliklere ve güvenlik güncellemelerine sahip olan [Microsoft Kimlik Doğrulama Kitaplığı'na (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) güncelleme yapmanızı öneririz.

Microsoft uygulamalarını kullanıyorsanız, Microsoft'un son destek bitiş tarihine kadar uygulamalarını MSAL'a geçmektedir ve MSAL'ın devam eden güvenlik ve özellik geliştirmelerinden yararlanacaklarından da temin edin.

1. [ADAL SSS bölümünü okuyunuz](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Uygulamaları platforma göre nasıl taşıyacağınız hakkında bilgi edinin](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Uygulamalardan hangilerinin ADAL'ı kullanabileceğini anlamanız için yardıma ihtiyacınız varsa tüm uygulamalarınızı kaynak kodunu gözden geçirmenizi ve varsa tüm ISV'lere veya uygulama sağlayıcılarına ulaşmanızı öneririz. Microsoft desteği ayrıca kiracınızdaki Microsoft dışı tüm ADAL uygulamalarının bir listesini de sağlayabilir.

**AAD Graph Geçişi**

Azure AD Graph kullanan uygulamalar için, Azure AD Graph uygulamalarını Microsoft Graph'e geçirme [yönergelerimizi izleyin.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Geçiş kontrol listemiz bir başlangıç noktası sağlar.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Azure uygulama kayıt portalınız, hangi uygulamaların AAD Graph kullandığını gösterir. Tüm uygulamalarınızın kaynak kodunu gözden geçirmenizi ve uygunsa, herhangi bir ISV veya uygulama sağlayıcıya ulaşmanızı öneririz. Microsoft desteği, kiracınız için tüm AAD Graph kullanımının bir listesini de sağlar.
3. Uygulamanın Microsoft Graph'te verilere erişmesi için, kullanıcı veya yöneticinin izin süreci aracılığıyla ona doğru izinleri ataması gerekir. [Microsoft Graph izinleri başvurusu,](https://docs.microsoft.com/graph/permissions-reference) her bir önemli Microsoft Graph API'leri kümesiyle ilişkilendirilmiş izinleri listeler. Ayrıca, izinleri kullanma konusunda da yol göstermeyi sağlar.
