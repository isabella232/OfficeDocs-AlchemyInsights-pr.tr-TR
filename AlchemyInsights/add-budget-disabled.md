---
title: Neden benim için bütçe Ekle düğmesi devre dışı?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807673"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Neden benim için bütçe Ekle düğmesi devre dışı?

Bütçe oluşturmak için aşağıdaki izinlerden birine ihtiyacınız vardır:

- Yönetim grubu, abonelik, kaynak grubu kapsamları
- Maliyet yönetimi Katılımcısı
- Kullanıcıya
- Katılımcı
- Yalnızca kurumsal müşteri: kayıt, departman, hesap kapsamları
- Kayıt Yöneticisi (kayıt kapsamında bütçe ayarlama)
- Bölüm Yöneticisi (Bölüm kapsamındaki bütçeyi ayarlama)
- Hesap sahibi (hesap kapsamındaki bütçeyi ayarlama)
- Yalnızca modern müşteri anlaşması: fatura hesabı, fatura profili, fatura bölümü kapsamları
- Azure aboneliği Oluşturucusu

**Geçerli aya ait maliyetlerim halen bütçelerimde bir bütçe oluşturdum. Neden uyarı almıyorum?**  
Uyarının işletilmez bir bütçe oluşturduğunuzda belirli bir maliyet eşiğini zaten aştıysanız. Yeni bir döngüden sonra, eşiği ihlal ederseniz uyarı başlatılır.

**Tanımlı bütçe uyarısı eşiklerimin birini aştığında uyarı almayı ne zaman beklemeli?**  
Bütçeler 4 saatte bir değerlendirilir. Kullanım verilerinin bütçe sistemine erişebilmesi için en az 8 saat sürer. Bu, bir eşiği aşmanızın ardından, uyarıların tetiklenmesi 12 saat kadar uzun sürebilir.

**Ay veya faturalandırma ay sıfırlama dönemi seçerken başlangıç tarihi düğmesi neden devre dışı?**  
Bütçeler geçerli takvim ayına veya geçerli fatura dönemine hizalanır (Faturalanan ay seçildiğinde). Bu nedenle bu değer sizin için önceden doldurulur.

**Bütçe oluşturma deneyiminde neden maliyetlerim 'in grafiğini görmüyorum?**  
Bütçe oluştururken size yardımcı olacak bir grafik işleyebilmek için en az 2 aylık maliyet verisi gerekir.

**Henüz bir bütçeyi henüz oluşturduğum bir aboneliğe göre ayarlayamıyorum?**  
Abonelik oluşturulduktan sonra, veriler bütçeyi ayarlamadan 24-48 saat sürer.

**Bütçe API kaynakları**

- [Bütçe API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): bütçeleri oluşturma ve güncelleştirme işlemlerini sağlar. Bütçe API 'sini kullanarak, bir bütçe eşiği ayarlayabilir ve bu eşiğe yaklaşıdıkça harekete geçmek için birden çok uyarı yapılandırabilirsiniz. Uyarılar, Otomasyonu gerçekleştirmek için e-posta veya Azure eylem grubunu tetikleyebilir. Not: Bu API için filtre uygulama, sorgu API filtresi/boyutları ile hizalanmaz.
- [Bütçeler API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): v1 'den daha yüksek maliyet filtreleme yeteneklerine sahip bütçeler oluşturun. Filtreleme, sorgu ve boyutlar API 'Lerinde kullanılan sözleşmeye hizalanır. Bu, ileriye doğru taşımayı kullanmak için önerilen bütçeler API 'dır.
- [Boyutlar](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): kullanımınız için çeşitli kapsamlar altında desteklenen boyutlara ulaşmak için işlemler sağlar. Boyutlar API 'sini kullanarak, sorgu API ile sorgu oluşturmaya yönelik giriş olarak kullanılabilecek boyutların listesini alabilirsiniz.
- [Sorgu](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): sağladığınız sorguya göre toplanmış maliyet ve kullanım verilerini almak için işlemler sağlar. Sorgu API 'sini kullanarak, istediğiniz tüm boyutlarda (Boyutlar API 'sinden erişilen) istediğiniz filtreleme, sıralama ve gruplandırma işlemlerini belirtebilirsiniz.

**Tahmin edilen maliyetler**

**Neden maliyetlerim için tahminleri maliyet analizinde göremiyorum?**  
Tahmin projeksiyonunun maliyet analizinde olmasının birden çok nedeni vardır, bunların bazıları aşağıdaki gibidir:

1. Maliyet verileriniz 10 günden azsa, tahmin grafiği yüklenmez. Model doğru tahminler için en az 10 günlük maliyet verisi gerektirir
2. Geçmişe ait tarihleri seçtiyseniz, tahmin grafiği görünür olmaz. Lütfen görüntülenecek tahmin grafiği için gelecek tarihleri içeren bir tarih aralığı seçin
3. Hesabınızda birden çok para birimi varsa, tahmin grafiği ' yalnızca ABD Doları olan tüm maliyetlerin maliyetleri gösterilir.

**Kaynaklarıma değişiklik yaptığımda neden tahmin değişikliği olmuyor?**  
Tahmin modeli, hesaptaki değişiklikleri hesaba eklemek için birkaç gün gerektirir ve kaynaklardaki değişikliklere dayalı olarak hemen bir projeksiyonu etkilemez  
Kaynaklarda artış veya azalma adımları için, modelin bu değişikliklere karşı daha uzun sürmesiyle

**Rezervasyonu veya Market satın aldıktan sonra tahminim neden artırım?**  
Tahmin modeli ' fiili maliyet ' bilgilerinizi dikkate alır ve kullanım ve satın alma için ayrı ayrı hesap yapmaz. Tek seferlik satın alma için, model, maliyette ani artış

**Tek bir boyutun tahminlerini görmek istiyorum (örn. Sayacı**  
Tahmin şu anda toplam maliyet tahminlerini destekler ve metre metre boyunca değildir. Dolayısıyla, ' boyuta göre gruplandırılmış olarak, tahminler boyut içindeki tüm maddelerin toplamı için olur

**Önerilen belgeler**

- [Azure maliyet yönetimi nedir?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure maliyet yönetimi en iyi yöntemleri](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Maliyetlerinizi ve harcamalarınızı çözümleme](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Maliyet analiziyle maliyetleri keşfetme ve çözümleme](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure maliyet yönetimi: fiyatlandırma](https://azure.microsoft.com/services/cost-management/#pricing)
- [Maliyet analizinde maliyetleri gözden geçirme](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video öğreticisi: Azure portalında bütçe oluşturma](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Bütçeleri görüntüleme ve özelleştirme önkoşulları](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Bütçe oluşturma ve yönetme](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Azure eylem gruplarıyla ve bütçeler API 'SI ile Otomasyonu yapılandırma](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Kullanım ve harcama izlemek için maliyet uyarılarını kullanma](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Maliyet yönetiminin en iyi yöntemleri](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Öğretici Videoları**

- [Azure portalında bütçe oluşturma](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Bütçeler API 'SI ve eylem gruplarıyla maliyetleri yönetme](https://go.microsoft.com/fwlink/?linkid=2147038)