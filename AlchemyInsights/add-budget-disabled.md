---
title: Bütçe ekle düğmesi benim için neden devre dışı?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954711"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Bütçe ekle düğmesi benim için neden devre dışı?

Bütçe oluşturmak için aşağıdaki izinlerden birini gerekir:

- Yönetim Grubu, Abonelik, Kaynak Grubu Kapsamları
- Maliyet Yönetimi Katkıda Bulunan
- Sahip
- Katkıda Bulunan
- Enterprise Yalnızca Müşteri: Kayıt, Bölüm, Hesap Kapsamları
- Kayıt Yöneticisi (Bütçeyi Kayıt kapsamına göre ayarlama)
- Bölüm Yöneticisi (Bütçeyi Bölüm kapsamına göre ayarlama)
- Hesap Sahibi (Bütçeyi Hesap kapsamına göre ayarlama)
- Yalnızca Modern Müşteri Sözleşmesi: Fatura Hesabı, Fatura Profili, Fatura Bölümü Kapsamları
- Azure abonelik oluşturucusu

**Geçerli ayın maliyeti zaten bütçeyi alamıyorken bir bütçe oluşturdum. Neden uyarı ala değilim?**  
Bütçe 2013 için uyarı oluştursanız bile bu uyarıyı oluşturmayacak şekilde, verilen maliyet eşiğini zaten aşmış durumda olursanız. Yeni bir döngü başladıktan sonra, eşiği ihlal edersiniz uyarı tetikler.

**Tanımlanan bütçe uyarı eşiklerinden birini aştırdikten sonra ne zaman bir uyarı alalım?**  
Bütçeler her 4 saatte bir değerlendirilir. Kullanım verileriyle bütçe sistemine ulaşmak en az 8 saat sürer. Bu nedenle, uyarıların bir eşiği aştırmanız 12 saat kadar sürebilir.

**Bir Ay veya Fatura ayı sıfırlama dönemi seçerek Başlangıç tarihi düğmesini neden devre dışı bırakılmıştır?**  
Bütçeler geçerli takvim ayı veya geçerli faturalandırma dönemine (Fatura Ay'ın seçili olduğu durumda) göre hizalanır. Bu nedenle, bu değeri sizin için önceden doldurmakta çalışıyoruz.

**Bütçe oluşturma deneyiminde neden maliyetlerimin grafiğini göremiyorum?**  
Bütçe oluşturma konusunda size yardımcı olacak bir grafik oluşturamadan önce en az 2 aylık maliyet verilerine ihtiyacımız var.

**Yeni oluşturduğum bir abonelik için neden bütçe ayarlay bilmiyorum?**  
Abonelik oluşturulmasının ardından, veriler buna göre bir bütçe ayarlamadan önce 24-48 saat sürer.

**Bütçe API Kaynakları**

- [Bütçeler API'si v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Bütçe oluşturmak ve güncelleştirmek için işlemler sağlar. Bütçeler API'sini kullanarak bir bütçe eşiği oluşturabilir ve bu eşik yaklaşıldığında tetiklanacak birden çok uyarı yapılandırabilirsiniz. Uyarılar, otomasyon gerçekleştirmek için e-postayı veya Azure Eylem Grubunu tetikler. Not: Bu API için filtreleme, Sorgu API'si filtrelemesi / boyutlarıyla uyumlu değildir.
- [Bütçeler API'si v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): v1'den daha yüksek maliyet filtreleme özellikleriyle bütçeler oluşturun. Filtreleme, Sorgu ve Boyutlar API'lerde kullanılan sözleşmeye göre hizalanır. Bu, ilerlemeyi kullanmak için önerilen bütçe API'sidir.
- [Boyutlar](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): Çeşitli kapsamlar kapsamında kullanımınız için desteklenen boyutlar elde etmek için işlemler sağlar. Boyutlar API'sini kullanarak, Sorgu API'si ile sorgu oluşturmak için giriş olarak kullanılan boyutların listesini elde edin.
- [Sorgu:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Sağladığınuz sorguya dayalı olarak toplanan maliyet ve kullanım verilerini almak için işlemler sağlar. Sorgu API'sini kullanarak, istediğiniz filtreleme, sıralama ve gruplamayı tüm kullanılabilir boyutlara (Boyutlar API'den erişilir) belirtebilirsiniz.

**Tahmini Maliyetler**

**Maliyet Çözümlemesi'ne neden maliyetlerim için tahminler göremiyorum?**  
Tahmin çözümlemesinde tahmin tahminlerinin sizin için eksik olması için birden çok neden vardır; bazıları şunlardır:

1. Maliyet verileriniz 10 günlükten azsa, tahmin grafiği yüklenmez. Model doğru projeksiyonlar için en az 10 günlük son maliyet verileri gerektirir
2. Tarihi tarihler seçtiysanız, tahmin grafiği görünmez. Tahmin grafiği için gelecek tarihler görüntülenecek olan bir tarih aralığı seçin
3. Hesabınız birden çok para birimine sahipse, tahmin grafiği 'USD'de tüm maliyetler' için yalnızca proje maliyetlerine sahip olur

**Kaynaklarımda değişiklik yapınca tahmin değişikliği neden değiştirmiyor?**  
Tahmin modelinin hesapta yapılan değişiklikleri hesaba yansıtması için birkaç gün gerekir ve kaynaklarda yapılan değişikliklere dayalı olarak acil projeksiyonlar yapmaz  
Kaynaklarda büyük bir artış veya düşüş adımları için modelin bu değişikliklere biraz daha uzun süreyle ayarlanması gerekir.

**Rezervasyon veya Market satın alma sonrasında tahminim neden artır oluyor?**  
Tahmin modeli 'Gerçek Maliyetinizi' göz önünde bulundurarak, kullanımı ve satın almaları ayrı olarak hesaba bağlı olarak değerlendirmez. Tek bir satın alma için model, maliyetlerdeki daha büyük bir artışa hesap yapmak için tahminleri 10 gün sonra azaltacaktır.

**Tek bir boyuta (ör. tahminler) görmek istiyorum. Metre)**  
Tahmin şu anda tek tek metreler için değil toplam maliyet tahminlerini destekler. Dolayısıyla, bir boyuta göre 'Gruplandı' olduğunda projeksiyonlar, boyuttaki tüm öğelerin toplamı için kullanılır

**Önerilen Belgeler**

- [Azure Maliyet Yönetimi nedir?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Maliyet Yönetimi en iyi yöntemleri](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Maliyetlerinizi ve harcamalarınızı çözümleme](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Maliyet çözümlemesi ile maliyetleri keşfetme ve çözümleme](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Maliyet Yönetimi: Fiyatlandırma](https://azure.microsoft.com/services/cost-management/#pricing)
- [Maliyet çözümlemesinde maliyetleri gözden geçirme](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video öğreticisi: Azure portalda bütçe oluşturma](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Bütçeleri görüntüleme ve özelleştirme için önkoşullar](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Bütçe oluşturma ve yönetme](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Azure Eylem Grupları ve Bütçeler API'si ile otomasyonu yapılandırma](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Kullanım ve harcamayı izlemek için maliyet uyarılarını kullanma](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Maliyet Yönetimi en iyi yöntemleri](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Öğretici videolar**

- [Azure portalda bütçe oluşturma](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Bütçeler API'si ve Eylem Grupları ile maliyetleri yönetme](https://go.microsoft.com/fwlink/?linkid=2147038)