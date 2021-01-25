---
title: Microsoft Graph API 'YI sorgulama
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
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974689"
---
# <a name="querying-the-microsoft-graph-api"></a>Microsoft Graph API 'YI sorgulama

Bu konu, hala Azure AD grafik API 'sini kullanan geliştiriciler için de geçerlidir. Ancak, tüm dizin, kimlik ve erişim yönetimi senaryolarınız için Microsoft Graph kullanmanız **kesinlikle** önerilir.

**Kimlik doğrulama veya yetkilendirme sorunları**

- Uygulamanız Microsoft Graph 'ı aramak için **belirteçleri edinemiyorsanız** , bu konuda daha belirli yardım ve destek almak için **erişim belirteci (kimlik doğrulama) alma hakkında sorun** seçin.
- Uygulamanız Microsoft Graph 'ı ararken **401 veya 403 yetkilendirme hataları** alıyorsa, bu konuda daha ayrıntılı yardım almak için **erişim reddedildi hatasını alma (yetkilendirme)** Microsoft Graph API kategorisini seçin.

**Microsoft Graph 'ı kullanmak istiyorum, ancak nereden başlayacağınızdan emin değil**

Microsoft Graph hakkında daha fazla bilgi edinmek için bkz:

- [Microsoft Graph 'a genel bakış](https://docs.microsoft.com/graph/overview)
- [Microsoft Graph 'ta kimlik ve erişim yönetimine genel bakış](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph uygulamalarını oluşturmaya başlarken](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** -kiracınızdaki veya bir tanıtım kiracısındaki Microsoft Graph API 'lerini test edin

**Microsoft Graph 'ı kullanmak istiyorum, ancak ihtiyacım olan v 1.0 Dizin API 'Lerini destekliyor mu?**

Microsoft Graph, dizin, kimlik ve erişim yönetimi için önerilen API 'dır. Ancak, Azure AD Graph ve Microsoft Graph 'ta mümkün olduğunca birkaç boşluk vardır. Seçiminize yardımcı olmak için en güncel farklılıkları vurgulayan aşağıdaki makaleleri gözden geçirin:

- [Azure AD grafiği ile Microsoft Graph arasındaki kaynak türü farklılıkları](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graph ve Microsoft Graph arasındaki özellik farklılıkları](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD ve Microsoft Graph arasındaki yöntem farklılıkları](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

***Kullanıcı* nesnesini sorgulıyorum, özelliklerinin çoğu eksik**

`GET https://graph.microsoft.com/v1.0/users` Microsoft Graph, döndürülecek varsayılan *Kullanıcı* özellikleri kümesini otomatik olarak seçtiği için, yalnızca 11 özellik verir. Başka *Kullanıcı* özelliklerine ihtiyaç duyarsanız, uygulamanızın ihtiyaç duyduğu özellikleri seçmek için $Select kullanın. Önce **Microsoft Graph Explorer** 'da deneyin.

**Bazı Kullanıcı özelliği değerleri, ayarladığım bilinmekle aynı şekilde *null***

En büyük olasılık açıklaması, uygulamaya kullanıcının verilmesinden kaynaklanır *. Readbasıc. All* izni. Bu, uygulamanın daha önce ayarlamış olsalar bile tüm diğer özellikleri null olarak döndürmesinin, sınırlı Kullanıcı özellikleri kümesini okumasına olanak tanır. Uygulama *kullanıcısına* izin vermeyi deneyin.

Daha fazla bilgi için [Microsoft Graph Kullanıcı izinleri](https://docs.microsoft.com/graph/permissions-reference#user-permissions)konusuna bakın.

**İsteklerim 'deki verileri filtrelemek için OData sorgu parametrelerini kullanırken sorun yaşıyorum**

Microsoft Graph, çok sayıda OData sorgu parametresini destekleirken, bu parametrelerin çoğu Microsoft Graph 'ta Dizin Hizmetleri ( *Directoryobject*'den devralan kaynaklar) tarafından tam olarak desteklenmez. Microsoft Graph 'ta, Azure AD grafiğinde bulunan sınırlamalar da korunur:

1. **Desteklenmiyor**: *null* veya *olmayan* null değerleri $Count, $Search ve $Filter
2. **Desteklenmiyor**: belirli özelliklerde $Filter (hangi özelliklere filtre uygulanamayacak kaynak konularına bakın)
3. **Desteklenmiyor**: sayfalandırma, filtreleme ve aynı anda sıralama
4. **Desteklenmiyor**: ilişkide filtreleme. Örneğin, İngiltere grubunun İngiltere 'deki tüm üyelerini bulun.
5. **Kısmi destek**: *kullanıcıya* $OrderBy (yalnızca DisplayName ve UserPrincipalName) ve *Grup*
6. **Kısmi destek**: $Filter (tek bir nesnenin ilişkilerini yalnızca *EQ* *,* *StartsWith*, *and ve* Limited *)* desteği, $Expand (tek nesnenin ilişkilerini genişletme tüm ilişkileri döndürür, ancak nesnelerin ilişkilerinin bir koleksiyonunu genişletme sınırlıdır)

Daha fazla bilgi [için bkz.](https://docs.microsoft.com/graph/query-parameters)

**Aradığım API çalışmıyor-daha fazla testi nasıl yapabilirim?**

**Microsoft Graph Explorer** -kiracınızdaki veya bir gösteri kiracısındaki Microsoft Graph API 'lerini test edin ve Microsoft Graph Explorer 'daki **örnek sorguları** inceleyin.

**Verileri sorgulıyorum ancak tamamlanmamış bir veri kümesi aldığımda**

Bir koleksiyonu sorgulamakta ( *Kullanıcılar* gibi), Microsoft Graph sunucu tarafı sayfa sınırlarını kullanır, böylece sonuçlar her zaman varsayılan sayfa boyutuyla döndürülür. Uygulamanız her zaman hizmetten gelen koleksiyonlar aracılığıyla Page 'i beklemelidir.

Daha fazla bilgi için bkz.:

- [Microsoft Graph en iyi uygulamalar](https://docs.microsoft.com/graph/best-practices-concept)
- [Uygulamanızda Microsoft Graph verilerini sayfalama](https://docs.microsoft.com/graph/paging)

**Uygulamam çok yavaş ve aynı zamanda daraltıldı. Hangi geliştirmeleri yapabilirim?**

Senaryonuza bağlı olarak, uygulamanızı daha iyi hale getirmek için ve bazı durumlarda hizmet tarafından daraltıldı (çok fazla arama yaparken) daha ucuz bir dizi farklı seçenek vardır.

Daha fazla bilgi için şu makalelere bakın:

- [Microsoft Graph en iyi uygulamalar](https://docs.microsoft.com/graph/best-practices-concept)
- [İstekleri toplu işleme](https://docs.microsoft.com/graph/json-batching)
- [Delta sorgusunda değişiklikleri izleme](https://docs.microsoft.com/graph/delta-query-overview)
- [Web kancaları aracılığıyla değişiklikleri öğrenin](https://docs.microsoft.com/graph/webhooks)
- [Azaltma Kılavuzu](https://docs.microsoft.com/graph/throttling)

**Hatalar ve bilinen sorunlar hakkında daha fazla bilgiyi nerede bulabilirim?**

- [Microsoft Graph hata yanıtı bilgileri](https://docs.microsoft.com/graph/errors)
- [Microsoft Graph ile ilgili bilinen sorunlar](https://docs.microsoft.com/graph/known-issues)

**Hizmet kullanılabilirliği ve bağlantısının durumunu nereden denetleyebilirim?**

Microsoft Graph aracılığıyla erişilebilecek temel hizmetlerin hizmet kullanılabilirliği ve bağlantısı, Microsoft Graph 'ın genel kullanılabilirliğini ve performansını etkileyebilir.

- Azure Active Directory hizmeti durumu için, [Azure durum sayfasında](https://azure.microsoft.com/status/)listelenen **güvenlik + kimlik** hizmetlerinin durumunu denetleyin.
- Microsoft Graph 'a katkıda bulunan Office Hizmetleri için, [Office hizmet durumu panosunda](https://portal.office.com/adminportal/home#/servicehealth)listelenen hizmetlerin durumunu denetleyin.
