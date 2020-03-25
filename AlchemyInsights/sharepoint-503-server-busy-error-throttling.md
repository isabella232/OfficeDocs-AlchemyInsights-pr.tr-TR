---
title: SharePoint Online Azaltma
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931246"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Online Azaltma

**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor. Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır. Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.

Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık. Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz. Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.

**503 sunucu meşgul hata**

Kullanıcılar SharePoint veya OneDrive sitelerine gezinmeye çalışırken bir 503 sunucu meşgul hata alabilir. 

Bu hata, SharePoint hizmeti içinde daraltma neden olabilir. SharePoint Online, SharePoint Online hizmetinin en iyi performansını ve güvenilirliğini korumak için azaltma yı kullanır. Azaltma, kaynakların aşırı kullanımını önlemek için kullanıcı eylemlerinin veya eşzamanlı çağrıların (komut dosyası veya koda göre) sayısını sınırlar. 

Azaltma hakkında daha fazla bilgi için [SharePoint Online'da daraltılmaktan veya engellenmesinden kaçının.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

Bu hatanın azaltmayla ilgisi olmadığını düşünüyorsanız, [İleti merkezi'ne](https://portal.office.com/adminportal/home#/MessageCenter)yönlendirerek kiracınızda etkin bir bakım olup olmadığını kontrol edebilirsiniz.

 Son olarak, oluşabilecek danışma/olayları kontrol etmek için [Hizmet Durumu](https://portal.office.com/adminportal/home#/servicehealth) sayfasını ziyaret ettiğinizden emin olun.

