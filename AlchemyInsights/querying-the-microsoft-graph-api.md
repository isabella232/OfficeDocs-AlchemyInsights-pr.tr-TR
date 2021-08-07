---
title: Microsoft Graph API'sini sorgulama
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
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923259"
---
# <a name="querying-the-microsoft-graph-api"></a>Microsoft Graph API'sini sorgulama

Bu konu, Hala Azure AD Graph API kullanan geliştiriciler için de geçerlidir. Bununla birlikte, **tüm dizin,** kimlik ve erişim yönetimi senaryolarınız Graph Microsoft Graph'i kullanmanız kesinlikle önerilir.

**Kimlik doğrulama veya yetkilendirme sorunları**

- Uygulamanız Microsoft  Graph'i aramak için belirteç alamasa da, bu konuda daha özel yardım ve destek almak için Microsoft Graph erişim belirteci **(Kimlik Doğrulama)** kategorisi alma ile ilgili sorun'u seçin.
- Uygulamanız Microsoft Graph'u arayarak arama sırasında **401 veya 403** yetkilendirme hatası alıyorsa, bu konuda daha özel yardım ve destek almak için Erişim reddedildi hatası **(Yetkilendirme)** Microsoft Graph API'si kategorisini seçin.

**Microsoft Graph'i kullanmak istiyorum ama nereden başlayacağımı bilmiyorum**

Microsoft Graph hakkında daha fazla bilgi için bkz:

- [Microsoft Graph'a genel bakış](https://docs.microsoft.com/graph/overview)
- [Microsoft Graph'ta Kimlik ve Erişim Yönetimi'ne genel Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph uygulamalarını Graph başlarken](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Kiracınız veya tanıtım Graph API'leri test etmek

**Microsoft Graph'i kullanmak istiyorum ama gereken v1.0 dizin API'lerini destekliyor mu?**

Microsoft Graph dizin, kimlik ve erişim yönetimi için önerilen API'dir. Bununla birlikte, Azure AD ad ve Microsoft Graph'da mümkün olan şeyler arasında hala birkaç Graph. Seçiminize yardımcı olacak en güncel farkları vurgulayan aşağıdaki makaleleri gözden geçirin:

- [Azure AD abonelikleri ile Microsoft Graph arasındaki kaynak türü Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD aboneliği ile Microsoft Graph arasındaki özellik Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD ile Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Kullanıcı nesnesini *sorgula* kullanılırken, özelliğin bir çoğu eksik**

`GET https://graph.microsoft.com/v1.0/users`Microsoft otomatik olarak, sonuç olarak Graph varsayılan kullanıcı özellikleri kümesi seçerken yalnızca 11 *özellik* döndürür. Diğer kullanıcı özelliklerine *ihtiyacınız* varsa, $select özellikleri seçmek için Diğer Özellikler'i kullanın. İlk olarak **Microsoft Graph Explorer'da** deneyin.

**Bazı kullanıcı özelliği *değerlerinin ayar* olduğunu bilse bile null**

Bunun en olası açıklaması, uygulamaya *User.ReadBasic.All izni verilmiş olmasıdır.* Bu, uygulamanın sınırlı bir kullanıcı özellikleri kümesi okumasine olanak sağlar ve daha önce ayarlanmış olsalar bile diğer tüm özellikleri null olarak döndürür. Bunun yerine *User.Read.All iznini uygulamayı* deneyin.

Daha fazla bilgi için [bkz. Microsoft Graph izinleri görüntüleme](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**İsteklerimde verileri filtrelemek için OData sorgu parametrelerini kullanırken sorunm var**

Microsoft Graph çok çeşitli OData sorgu parametrelerini desteklerken, bu parametrelerin birçoğu Microsoft Graph'te dizin hizmetleri *(dizinObject'den* devralan kaynaklar) tarafından tam olarak Graph. Azure AD'de var olan aynı sınırlamalar, Microsoft Graph'nin çoğu bölümünde Graph:

1. **Desteklenmiyor: $count,**$search ve $filter *null veya null* olmayan *değerlerle ilgili*
2. **Desteklenmiyor: bazı**$filter hakkında daha fazla bilgi (hangi özelliklerin filtrelenebilir olduğuyla ilgili kaynak konularına bakın)
3. **Desteklenmiyor:** aynı anda hem diskte hem filtreleme hem de sıralama
4. **Desteklenmiyor:** bir ilişkiye göre filtreleme. Örneğin - Birleşik Krallık'ta olan mühendislik grubunun tüm üyelerini bulun.
5. **Kısmi destek:**$orderby *(yalnızca* displayName ve userPrincipalName) ve *grupla* ilgili destek
6. **Kısmi destek:**$filter (yalnızca *eq*,  *ile* başlar , veya ve ve sınırlı ) desteği, $expand (tek bir nesnenin ilişkilerini genişletmek tüm ilişkileri döndürür, ancak nesnelerin ilişki koleksiyonunu genişletmek sınırlıdır)

Daha fazla bilgi için [bkz. Yanıtları sorgu parametreleriyle özelleştirme.](https://docs.microsoft.com/graph/query-parameters)

**Çağrı yapacağım API çalışmıyor, nereden daha fazla test yapabilirim?**

**Microsoft Graph Explorer** - Kiracı Graph veya tanıtım kiracısı olarak Microsoft Graph API'lerini test edin ve Microsoft Graph Explorer'daki örnek sorgulara göz atabilirsiniz. 

**Verileri sorgula kullanılırken eksik bir veri kümesi geliyor gibi görünüyor**

Bir koleksiyonu (kullanıcılar gibi) sorgularsanız, Microsoft Graph sunucu tarafı sayfa sınırlarını kullanır ve böylece sonuçlar her zaman varsayılan sayfa boyutuyla döndürülür. Uygulama her zaman hizmetten döndürülen koleksiyonlar boyunca sayfayı atlar.

Daha fazla bilgi için bkz.:

- [Microsoft Graph yöntemleri](https://docs.microsoft.com/graph/best-practices-concept)
- [Microsoft'u Graph verileriyle çevrimiçi olarak çevrimiçi çalışma](https://docs.microsoft.com/graph/paging)

**Uygulamam çok yavaş ve aynı zamanda kısıtlanıyor. Hangi geliştirmeleri ben sağlarim?**

Senaryonıza bağlı olarak, uygulamanızı daha iyi performans ortaya çıkarmanız için ve bazı durumlarda (çok fazla arama yaparken) hizmet tarafından azaltmaya daha az az neden olan çeşitli seçenekler vardır.

Daha fazla bilgi için şu makalelere bakın:

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
