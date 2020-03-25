---
title: 503 hatayla sharePoint geçişi azaltma
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931678"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a>503 hatayla sharePoint geçişi azaltma

**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor. Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır. Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.

Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık. Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz. Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.

**SharePoint Online'a geçiş yaparken 503 hata**

SharePoint Online'a geçiş yapıyor ve 503 hata alıyor gibi görünüyor. Lütfen aşağıdaki adımları uygulayın, böylece size en kısa sürede yardımcı olabiliriz. 

1. **Destekle İlgili İletişim'i**ve ardından **Yeni Hizmet İsteği'ni**tıklatın.
2. Başlık ve açıklama için **SharePoint Geçiş Azaltma yazısını 503 ile**.
3. Bilet gönderildikten sonra, lütfen aşağıdaki bilgilerle güncelleyin:
    - Geçişin ne kadarı kaldı (örneğin, kaç TB?).
    - Geçiş başlangıç ve bitiş tarihi.
    - SharePoint Server, Box, GDrive, File shares, vb. gibi içeriğinizi nereden geçirdiğinizi açıklayın.
    - Azaltma hatalarının sayısını (örneğin, saatte x azaltma?) ve azaltma ne zaman gerçekleştiğini tahmin edin.
    - Hangi geçiş aracını kullanıyorsunuz (örneğin, SPMT veya ShareGate).


