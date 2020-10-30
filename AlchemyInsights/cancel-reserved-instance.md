---
title: Rezervasyonu iptal etme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807986"
---
# <a name="cancelling-reservation"></a>Rezervasyonu iptal etme

- **Self servis:** Ayrılmış bir örneği [Azure portalı](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)kullanarak kendiniz iptal edebilir veya değiştirebilirsiniz. Rezervasyonu seçin ve geri ödeme veya Exchange 'e tıklayın. Exchange veya geri ödeme yapmak için, rezervasyon emrinde sahip erişiminizin olması gerektiğini unutmayın. Yalnızca rezervasyonun erişimi geri ödeme veya Exchange ile devam edemeyecektir. Rezervasyon siparişi sahibine, rezervasyon siparişine sahip size sahip erişiminizi vermesini isteyin
- **Exchange ilkesi:** Aynı türden başka bir rezervasyon için bir ayırma alışverişi yapabilirsiniz – rezervasyon alışverişi sırasında **hiçbir sorun olmaz** . Yeni rezervasyonun toplam taahhütler, değiştirilen rezervasyonun geri ödeme tutarının ve gelecekteki aylık ödemelerin (uygunsa) sayısından büyük olmalıdır
- Geri **ödeme ilkesi:** Geri ödeme toplamı ve iptal edilen gelecek ödemeler 12 aylık yuvarlama penceresinde $50.000 USD 'yi aşamaz. Şu anda para iadelerinize **herhangi bir cezası** ücretsizdir, ancak gelecekteki geri iadede ücretlendirilir  
    **Özel durumlar:** ABD hükümeti Kurumsal Sözleşme müşterileri için self servis alışverişi ve iptal özelliği kullanılamaz
- **API/PS/CLI** desteği iptal etme ve geri ödeme için [self servis alışverişleri ve Azure ayırmaları için geri ödemeler](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) için kullanılamaz
- ABD hükümeti Kurumsal Sözleşme müşterileri için self servis alışverişi ve iptal yeteneği kullanılamaz. Kullandıkça öde ve CSP gibi ABD kamu aboneliği türleri desteklenmektedir

Daha fazla bilgi: [İade ve Exchange Işlemleri nasıl işlenir](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Daha fazla bilgi: [Exchange ve geri ödeme ilkeleri](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Diğer sorular: [ayrılmış örnek belgelerini ziyaret edin](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Var olan ayrılmış bir örneği (self servis) değiştirme**

Aynı türden başka bir rezervasyon için rezervasyonu değiştirebilirsiniz. Artık ihtiyaç duymuyorsa, bir rezervasyonu para, $50.000 ABD Doları kadar ayarlayabilirsiniz. ABD hükümeti Kurumsal Sözleşme müşterileri için self servis alışverişi ve iptal yeteneği kullanılamaz. Kullandıkça öde ve CSP gibi ABD kamu aboneliği türleri desteklenmektedir. Var olan rezervasyonu alışverişi veya geri ödemeniz için, rezervasyon emrinde sahip erişiminizin olması gerekir.

Aşağıdaki adımlar işlemi tamamlamaya yardımcı olur

1. [Azure portalınızda](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)oturum açın. Geri ödeme yapmak istediğiniz rezervasyonları seçin ve **Exchange** 'e tıklayın
2. Satın almak istediğiniz VM ürününü seçin ve bir miktar yazın. Yeni [Satınalma toplamının iade toplamı 'ndan](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy) daha fazla olduğundan emin olun
3. İşlemi gözden geçirme ve tamamlama

**Ayrılmış bir örnek için geri ödeme**

Rezervasyonu geri vermek için, **rezervasyon ayrıntılarına** gidin ve geri **ödeme** 'yi tıklatın

**Proforma para iadesi:**

**Para iadesi ve Kambiyo için proforma ve minimum gereksinim örnekleri**  
Upfront RESERVATION örneği:

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

**Önerilen belgeler**

- [İade ve Exchange işlemleri nasıl işlenir](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Exchange ve geri ödeme ilkeleri](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)