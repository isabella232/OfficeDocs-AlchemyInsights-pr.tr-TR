---
title: Rezervasyon iptal edildi
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 8d0a6a37a244e817472c3949109481a30d80328b7353806905e05c547e196ea0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931253"
---
# <a name="cancelling-reservation"></a>Rezervasyon iptal edildi

- **Self servis:** Azure portalını kullanarak özel kullanım örneklerini iptal edebilir veya özel kullanım için [değiştirme işlemi kullanabilirsiniz.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Rezervasyon seçin ve para iadesine veya değişime tıklayın. Değiştirme veya para iadesi yapmak için Rezervasyon Siparişi'ne sahip erişiminiz olması gerektiğini unutmayın. Yalnızca Rezervasyona erişim, para iadesi veya değişim ile devam edebilirsiniz. Rezervasyon Siparişi sahibinden size Rezervasyon Siparişine sahip erişimi vermelerini iste
- **Exchange ilke:** Aynı türde başka bir rezervasyon için rezervasyon alışverişi yaptırabilirsiniz, rezervasyon **değiştirmesinde hiçbir** penaltı yoktur. Yeni rezervasyonla ilgili toplam taahhüt, değişten rezervasyon tutarının toplamından ve gelecekte yapılacak aylık ödemelerden (uygunsa) daha fazla olmalıdır
- **İade politikası:** İade toplamı ve iptal edilen gelecekteki ödemeler 12 aylık ödeme penceresinde 50.000 ABD Doları'nın üzerinde olamaz. Şu anda **para iadeleri için herhangi bir** ücret tahsil edilmİstir, ancak gelecekte yapılacak para iadeleri için ücretlendirmeyi  
    **Özel Durumlar:** ABD Kamu müşterileri, self servis değiştirme ve iptal Kurumsal Anlaşma kullanılamıyor
- **API / PS / CLI** desteği iptal ve geri ödemelerde Self servis alışveriş ve Azure Rezervasyonları için geri ödeme [kullanılamaz](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- ABD Kamu müşterileri, self servis değiştirme ve iptal Kurumsal Anlaşma kullanılamıyor. Pay-As-You-Go ve CSP gibi diğer ABD Kamu abonelik türleri de destekle

Daha fazla bilgi: [İade ve değiştirme işlemleri nasıl işlenir?](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Daha fazla bilgi: [Exchange ve Para iadesi ilkeleri](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Diğer sorular: [Özel kullanım örneği belgelerini ziyaret edin](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange özel kullanım örneği (Self Servis)**

Aynı türde başka bir rezervasyon için rezervasyon alışverişi yaptırabilirsiniz. Ayrıca, artık ihtiyacınız yoksa yıllık 50.000 ABD Doları'nın üzerinde bir rezervasyon için para iadesi alabilirsiniz. ABD Kamu müşterileri, self servis değiştirme ve iptal Kurumsal Anlaşma kullanılamıyor. Pay-As-You-Go ve CSP gibi diğer ABD Kamu abonelik türleri de desteklene. Mevcut bir rezervasyonu değiştirmek veya iade etmek için Rezervasyon Siparişi'ne sahip erişiminiz olmalıdır.

Aşağıdaki adımlar, işlemi tamamlamak için yordamda yol gösterir

1. [Azure portalda oturum açın.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) geri ödeme yapmak istediğiniz rezervasyonları seçin ve Rezervasyonlar'a **Exchange**
2. Satın almak istediğiniz sanal makine ürününü seçin ve bir miktar yazın. Yeni satın alma toplamının iade toplamının üzerinde olduğundan emin olun Satın alma [öncesinde doğru boyutu belirleme](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. İşlemleri gözden geçirme ve tamamlama

**Ayrılmış bir örnek için para iadesi**

Bir rezervasyonu geri ödemek için Rezervasyon **Ayrıntıları'ne gidin ve Geri** Ödeme'ye **tıklayın**

**Pro dereceli para iadesi:**

**Pro ve değiştirme için en düşük gereksinim örnekleri**  
Upfront rezervasyon örneği:

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

**Önerilen Belgeler**

- [İade ve değiştirme işlemleri nasıl işlenir?](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Exchange ve Para İadesi ilkeleri](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)