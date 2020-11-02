---
title: Ayrılmış örnek satın alma Faturalaması
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
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823173"
---
# <a name="billing-for-reserved-instance-purchase"></a>Ayrılmış örnek satın alma Faturalaması

Rezerve edilmiş örnek satınalımı, satın alma sırasında seçtiğiniz aboneliğe bağlı ödeme yöntemine ücretlendirilir. Abonelik türü bir kurumsal anlaşma (teklif numarası: MS-AZR-0017P), bir iş yerinde Öde (teklif numarası: MS-AZR-0003P), Microsoft Müşteri Sözleşmesi veya CSP olmalıdır.

- Kurumsal abonelik için, giderlerin para taahhüdü bakiyesinden düşülür veya aşırı yaş olarak ücretlendirilmektedir
- Devam eden öde aboneliği için, ücretler, aboneliğin kredi kartı veya fatura ödemesi yöntemine faturalanır

**Rezervasyonu iptal etme**

- **Self servis:** Ayrılmış bir örneği [Azure portalı](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)kullanarak kendiniz iptal edebilir veya değiştirebilirsiniz. Rezervasyonu seçin ve geri ödeme veya Exchange 'e tıklayın. Exchange veya geri ödeme yapmak için, rezervasyon emrinde sahip erişiminizin olması gerektiğini unutmayın. Yalnızca rezervasyonun erişimi geri ödeme veya Exchange ile devam edemeyecektir. Rezervasyon siparişi sahibine, rezervasyon siparişine sahip size sahip erişiminizi vermesini isteyin
- **Exchange ilkesi:** Aynı türden başka bir rezervasyon için bir ayırma alışverişi yapabilirsiniz – rezervasyon alışverişi sırasında **hiçbir sorun olmaz** . Yeni rezervasyonun toplam taahhütler, değiştirilen rezervasyonun geri ödeme tutarının ve gelecekteki aylık ödemelerin (uygunsa) sayısından büyük olmalıdır
- Geri **ödeme ilkesi:** Geri ödeme toplamı ve iptal edilen gelecek ödemeler 12 aylık yuvarlama penceresinde $50.000 USD 'yi aşamaz. Şu anda para iadelerinize **herhangi bir cezası** ücretsizdir, ancak gelecekteki geri iadede ücretlendirilir

**Özel durumlar:** ABD hükümeti Kurumsal Sözleşme müşterileri için self servis alışverişi ve iptal özelliği kullanılamaz

- **API/PS/CLI** desteği iptal etme ve geri ödeme için [self servis alışverişleri ve Azure ayırmaları için geri ödemeler](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) için kullanılamaz
- ABD hükümeti Kurumsal Sözleşme müşterileri için self servis alışverişi ve iptal yeteneği kullanılamaz. Kullandıkça öde ve CSP gibi ABD kamu aboneliği türleri desteklenmektedir

Daha fazla bilgi edinin: [İade ve Exchange Işlemleri nasıl işlenir](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) daha fazla bilgi edinin: [Exchange ve geri ödeme ilkeleri](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) diğer sorular: [ayrılmış örnek belgeleri ziyaret edin](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Var olan ayrılmış bir örneği (self servis) değiştirme**

Aynı türden başka bir rezervasyon için rezervasyonu değiştirebilirsiniz. Artık ihtiyaç duymuyorsa, bir rezervasyonu para, $50.000 ABD Doları kadar ayarlayabilirsiniz. ABD hükümeti Kurumsal Sözleşme müşterileri için self servis alışverişi ve iptal yeteneği kullanılamaz. Kullandıkça öde ve CSP gibi ABD kamu aboneliği türleri desteklenmektedir. Var olan rezervasyonu alışverişi veya geri ödemeniz için, rezervasyon emrinde sahip erişiminizin olması gerekir.

Aşağıdaki adımlar işlemi tamamlamaya yardımcı olur

1. [Azure portalınızda](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)oturum açın. Geri iadesi istediğiniz rezervasyonları seçin ve **Exchange** 2 ' ye tıklayın. satın almak istediğiniz VM ürününü seçin ve bir miktar yazın. Yeni satınalma toplamının, [satın alma öncesinde doğru boyutu saptamadan önce](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)iade toplamı
3. işlemi gözden geçirin ve tamamlayın

**Ayrılmış bir örnek için geri ödeme**

Rezervasyonu geri vermek için, **rezervasyon ayrıntılarına** gidin ve geri **ödeme** 'yi tıklatın

**Proforma para iadesi:**

**Para iadesi ve Kambiyo Için proforma ve minimum gereksinim örnekleri** Upfront RESERVATION örneği:

- $120 Ocak 'ta için tek yıllık bir dönem RI satın alabilirsiniz
- 7 Nisan tarihinde, bu rezervasyonu geri ödeme veya Exchange
- Rezervasyon 97 gündür canlı olduğundan, (1-97/365) * $120 geri alırsınız. (yani $88,1). Şu anda para iadelerimde ceza yok
- Alış verişi yapıyorsanız, yeni satın alma işleminizin $88,1 'tan büyük olması gerekir
- Şu anda para iadelerimde ceza yok

**Fatura planı rezervasyonu örneği:**

- Aylık $10 için tek yıllık bir dönem RI satın alabilirsiniz
- 7 Nisan tarihinde, bu rezervasyonu geri ödeme veya Exchange
- Son ödeme 7 gün gerçekleşti, (1-7/31) * $10 geri alırsınız. (yani $7,74)
- Gelecekteki ödemeler $80. Şu anda para iadelerimde ceza yok
- Bu İptalin $50.000 $87,74
- Alış verişi yapıyorsanız, yeni satınalmanın toplam değeri $87,74 ' dan büyük olmalıdır

**Son faturalandırma döneminin faturası göremiyor**

Fatura görmeyemeyeceğiniz bazı olası nedenler:

- Aboneliğiniz olan ve ücretsiz bir deneme süreniz olan aylık bir kontörünüz varsa. Fatura yalnızca para borcu oluşturulur
- Azure 'a abone olduğunuz günden 30 günden daha azdır
- Fatura henüz oluşturulmaz. Faturalandırma döneminin sonuna kadar bekle
- Hesap yöneticisi değilseniz, eski faturalar size uygun olmayabilir

**Faturanızı Azure portalından indirin (. PDF)**

- Azure portalında [abonelikler](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) sayfasından, [faturalara erişimi olan bir Kullanıcı](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support) olarak aboneliğinizi seçin
- **Faturaları** Seç
- PDF faturanızın bir kopyasını görüntülemek için **Fatura indir** 'e tıklayın. **Mevcut değilse** , [son faturalandırma dönemi için neden fatura göremiyorum?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Faturanızı e-postada (. PDF) alma**

- [Abonelikler](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) sayfasından aboneliğinizi seçin. **Faturalar** 'ı, ardından e-posta faturamı
- Kabul **et 'e tıklayın ve** koşulları kabul edin. Sahip olduğunuz her aboneliğe sahip olmanız gerekecektir

Not: adımları uyguladıktan sonra bir e-posta alamazsanız, [profilinizdeki iletişim tercihlerinde](https://account.windowsazure.com/profile) e-posta adresinizin doğru olduğundan emin olun

**Azure portalından kullanım verilerinizi indirin**

- [Hesap Yöneticisi](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) olarak [Azure Hesap Merkezi 'nde](https://account.windowsazure.com/Subscriptions) oturum açın
- Fatura ve kullanım bilgilerini istediğiniz aboneliği seçin
- **Faturalandırma geçmişini** seçin
- Tahminin oluşturulduğu sırada ücretlerinizi tahmin etmek için **geçerli Ifadeyi görüntüle** 'yi seçin
- Günlük kullanım verilerini CSV dosyası olarak indirmek için **kullanımı indir** 'i seçin. Kullanılabilir iki sürüm görürseniz, sürüm 2

Diğer sorular: [ayrılmış örnek belgelerini ziyaret edin](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Önerilen belgeler**

- [Faturalandırma temelleri](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Ayrılmış örnek iskontosunun nasıl uygulandığını anlama](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Faturalandırma faturasını ve günlük kullanım verilerinizi indirme veya görüntüleme](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Ayrılmış örnek iskontosunun nasıl uygulandığını anlama](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Yapılacaklar aboneliğiniz için ayrılmış örnek kullanımını anlama](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kurumsal kaydınız için ayrılmış örnek kullanımını anlama](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows yazılım ücretleri ayrılmış örneklere dahil değildir](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Iş Ortağı Merkezi bulut çözüm sağlayıcısı (CSP) programındaki ayrılmış örnekler](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)