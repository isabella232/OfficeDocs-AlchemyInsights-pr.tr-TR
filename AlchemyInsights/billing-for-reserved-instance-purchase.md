---
title: Özel Kullanım Örneği satın alımı için faturalama
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
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820342"
---
# <a name="billing-for-reserved-instance-purchase"></a>Özel Kullanım Örneği satın alımı için faturalama

Özel kullanım örneği satın alma, satın alma zamanında seçili olan aboneliğe bağlı ödeme yöntemi üzerinden tahsil edilecektir. Abonelik türü bir kurumsal sözleşme (teklif numarası: MS-AZR-0017P), Pay-As-You-Go (teklif numarası: MS-AZR-0003P), Microsoft Müşteri Sözleşmesi veya CSP olması gerekir.

- Kurumsal abonelik için ücretler kaydın para taahhüdü bakiyelerinden düşülebilir veya fazlalık olarak ücret alınacaktır.
- 'As-You-Go' aboneliği için ücretler abonelik üzerinden kredi kartına veya fatura ödeme yöntemine fatura gideri

**Rezervasyon iptal edildi**

- **Self servis:** Azure portalını kullanarak özel kullanım örneklerini iptal edebilir veya özel kullanım için [değiştirme işlemi kullanabilirsiniz.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Rezervasyon seçin ve para iadesine veya değişime tıklayın. Değiştirme veya para iadesi yapmak için Rezervasyon Siparişi'ne sahip erişiminiz olması gerektiğini unutmayın. Yalnızca Rezervasyona erişim, para iadesi veya değişim ile devam edebilirsiniz. Rezervasyon Siparişi sahibinden size Rezervasyon Siparişine sahip erişimi vermelerini iste
- **Exchange ilkesi:** Aynı türde başka bir rezervasyon için rezervasyon alışverişi yaptırabilirsiniz, rezervasyon **değiştirmesinde hiçbir** penaltı yoktur. Yeni rezervasyonla ilgili toplam taahhüt, değişten rezervasyon tutarının toplamından ve gelecekte yapılacak aylık ödemelerden (uygunsa) daha fazla olmalıdır
- **İade politikası:** İade toplamı ve iptal edilen gelecekteki ödemeler 12 aylık ödeme penceresinde 50.000 ABD Doları'nın üzerinde olamaz. Şu anda **para iadeleri için herhangi bir** ücret tahsil edilmİstir, ancak gelecekte yapılacak para iadeleri için ücretlendirmeyi

**Özel Durumlar:** ABD Kamu Kurumsal Sözleşme müşterileri self servis değiştirme ve iptal etme özelliğine sahip değildir

- **API / PS / CLI** desteği iptal ve geri ödemelerde Self servis alışveriş ve Azure Rezervasyonları için geri ödeme [kullanılamaz](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- ABD Kamu Kurumsal Sözleşme müşterileri self servis değiştirme ve iptal etme özelliğine sahip değildir. Pay-As-You-Go ve CSP gibi diğer ABD Kamu abonelik türleri de destekle

Daha fazla bilgi: [İade ve değiştirme işlemleri](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) nasıl işlenir Daha fazla bilgi : Exchange ve Para [İadesi ilkeleri](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Diğer sorular: Özel kullanım [belgeleri'ne ziyaret edin](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Var olan bir özel kullanım örneğini değiştirme (Self servis)**

Aynı türde başka bir rezervasyon için rezervasyon alışverişi yaptırabilirsiniz. Ayrıca, artık ihtiyacınız yoksa yıllık 50.000 ABD Doları'nın üzerinde bir rezervasyon için para iadesi alabilirsiniz. ABD Kamu Kurumsal Sözleşme müşterileri self servis değiştirme ve iptal etme özelliğine sahip değildir. Pay-As-You-Go ve CSP gibi diğer ABD Kamu abonelik türleri de desteklene. Mevcut bir rezervasyonu değiştirmek veya iade etmek için Rezervasyon Siparişi'ne sahip erişiminiz olmalıdır.

Aşağıdaki adımlar, işlemi tamamlamak için yordamda yol gösterir

1.Azure [portalında oturum açın.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) İade etmek istediğiniz rezervasyonları seçin ve **Exchange** 2'ye tıklayın.Satın almak istediğiniz VM ürününü seçin ve miktarı yazın. Yeni satın alma toplamının iade toplamının üzerinde olduğundan emin olun Satın alma [öncesinde doğru boyutu seçin.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.İşlemleri gözden geçirme ve tamamlama

**Ayrılmış bir örnek için para iadesi**

Bir rezervasyonu geri ödemek için Rezervasyon **Ayrıntıları'ne gidin ve Geri** Ödeme'ye **tıklayın**

**Profesyonel geri ödeme:**

**Geri ödeme ve değişim için artım ve minimum gereksinim örnekleri** Upfront rezervasyon örneği:

- 1 Ocak'ta 120 ABD Doları için bir yıllık RI satın alı
- 7 Nisan'da bu rezervasyonu geri ödemeniz veya değiştirmeniz gerekiyor
- Rezervasyon 97 gün boyunca canlı olarak yapıldıktan sonra (1-97/365) * 120 $ geri ödemesi elde edilir. (88,1 TL gibi). Şu anda geri ödemelerde bir sorun yok
- Alışveriş yaptıysanız, yeni alışverişin 88,1 TL'den büyük olması gerekir
- Şu anda geri ödemelerde sorun yok

**Fatura planı rezervasyon örneği:**

- Aylık 10 ABD Doları için bir yıllık RI satın alı
- 7 Nisan'da bu rezervasyonu geri ödemeniz veya değiştirmeniz gerekiyor
- Son ödeme 7 gün olduğu için size (31/1-7/31) * 10 TL geri ödemesi olur. (yani 7,74 TL)
- Gelecekte iptal edilen ödemeler 80 ABD Doları'dır. Şu anda geri ödemelerde bir sorun yok
- Bu iptal, 50.000 TL geri ödeme sınırınıza göre 87,74 TL'den düşecek
- Alışveriş yapılansa, yeni satın almaların toplam değeri 87,74 TL'den büyük olmalı

**Son faturalandırma dönemine göre fatura görmek mümkün değil**

Fatura görmeyebilirsiniz, bunun bazı olası nedenleri vardır:

- Aboneliğinizin süresi aşmadı veya Ücretsiz Deneme sürümüne sahip olduğunuz aylık kredi tutarınız var. Fatura, yalnızca para ödemesi yapılan ödeme olduğunda oluşturulur
- Azure'a abone olduğunuz günden 30 günden daha kısa bir süre
- Fatura henüz oluşturulmadı. Faturalandırma döneminin sonuna kadar bekleyin
- Hesap Yöneticisi değilseniz eski faturaları kullanabilirsiniz

**Faturanızı Azure portaldan (.pdf) indirin**

- Azure portalda [Abonelikler](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) sayfasından faturalara erişimi olan bir kullanıcı [olarak aboneliğinizi seçin](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- **Faturalar'ı seçin**
- PDF **faturanın bir** kopyasını görüntülemek için Faturayı İndir'e tıklayın. Kullanılamıyor **olarak yazıyorsa** [bkz. Son faturalandırma dönemi için neden fatura göremiyorum?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Faturanızı e-postayla (.pdf) alma**

- Abonelikler sayfasından [aboneliğinizi](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) seçin. **Faturalar'a ve sonra Faturamı** e-posta ile gönder'e tıklayın
- Kabul **et'e** tıklayın ve koşulları kabul et'e tıklayın. Sahibi olduğunuz her abonelik için katılmanız gerekir

Not: Adımları takipdikten sonra e-posta alasanız bile, profilinizde yer alan iletişim tercihlerinde e-posta [adresinizin doğru olduğundan emin olun](https://account.windowsazure.com/profile)

**Kullanım verilerinizi Azure portaldan indirme**

- Hesap Yöneticisi [olarak Azure Hesap Merkezi'nde](https://account.windowsazure.com/Subscriptions) oturum [açma](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Fatura ve kullanım bilgilerini istediğiniz aboneliği seçin
- Ödeme **Geçmişi'yi seçin**
- Geçerli **Bildirimi Görüntüle'yi** seçerek, tahminin oluşturulma zamanı içinde ücretlerin tahminini görmek için
- Günlük **kullanım verilerini** CSV dosyası olarak indirmek için Kullanımı İndir'i seçin. kullanılabilir iki sürüm görüyorsanız, 2. sürümü indirin

Diğer sorular: [Özel kullanım örneği belgelerini ziyaret edin](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Önerilen Belgeler**

- [Faturalamayla ilgili temel bilgiler](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Özel Kullanım Örneği indirimin nasıl uygulandığını anlama](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure faturanızı ve günlük kullanım verilerinizi indirme veya görüntüleme](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Özel Kullanım Örneği indirimin nasıl uygulandığını anlama](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kullanıda Öde aboneliğiniz için Özel Kullanım Örneği kullanımını anlama](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kurumsal kaydınız için Özel Kullanım Örneği kullanımını anlama](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Özel amaçlı örneklere dahil edilen Windows yazılım maliyetleri](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [İş Ortağı Merkezi Bulut Çözümü Sağlayıcısı (CSP) programında Özel Kullanım Örnekleri](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)