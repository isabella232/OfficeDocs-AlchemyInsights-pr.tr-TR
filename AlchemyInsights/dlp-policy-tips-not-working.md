---
title: DLP İlke İpuçları çalışmıyor
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932606"
---
# <a name="dlp-policy-tip-issues"></a>DLP İlke İpucu sorunları

**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor. Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır. Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.

Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık. Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz. Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.

**DLP ilke ipuçları**

**DLP ilkeleri**kullanırken, kullanıcılar **ilke ipuçları**ile bir ilke ihlali haberdar edilebilir. Yöneticiler, DLP ilkelerini sınarken veya ilke tam uygulama modundayken görüntülenecek ilke ipuçlarını yapılandırabilir.
  
Güvenlik ve Uyumluluk merkezindeki DLP ilkeniz hakkındaki ilke ipuçlarını tam uygulama modunda yapılandırmak için aşağıdakileri yapın:
  
- [Buradaki](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)adımları kullanarak DLP kuralında ilke ipuçlarının **etkinleştirildiğinden** emin olun.

- İçeriğinizin bu [makalede](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)özetlenen kuralı tetiklemek için **gerekenle** **eşleştiğinden** emin olun.

- İlke ipuçları hem OWA hem de Outlook'ta görüntülenir. Ancak, **Outlook 2013 veya daha sonra**kullanırken, ilke ipuçları yalnızca belirli koşullar altında görüntülenir. Bu koşullar burada listelenmiştir: [İlke İpuçlarını görüntülemek için Outlook 2013 veya sonraki](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions) koşullar

DLP ilke ipuçları hakkında daha fazla bilgi için bkz: [DLP İlkeleri için ilke ipuçlarını göster](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  