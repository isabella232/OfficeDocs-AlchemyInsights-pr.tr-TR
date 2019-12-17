---
title: Günlük e-posta sınırı aşıldı. İş akışı askıya alındı.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053137"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Günlük e-posta Sınırı Aşıldı. İş akışı askıya alındı.

Bu hata aşağıdaki senaryolarda alınabilir:

- SharePoint Online'da SharePoint 2010 veya SharePoint 2013 iş akışı platform türünü kullanan bir iş akışınız vardır.
- İş akışı, aynı anda 200'den fazla kullanıcıya, günde 10.000'den fazla alıcıya veya dakikada 30'dan fazla iletigöndermek üzere özel bir e-posta iletisi gönderecek şekilde yapılandırılmıştır.
- İş akışını çalıştırdığınızda, e-posta iletisi gönderilmez ve aşağıdaki davranışı fark e-postayla fark e-posta yla karşılarınız:
    - SharePoint 2013 platform türünü kullanan bir iş akışı için **İş Akışı Durumu** sayfasına göz atarsınız. İş Akışı Durumu sayfasında, **İç Durum** **Başlatıldı**olarak ayarlanır ve bilgi balonu **alıcıya gönderilemeyince**görüntülenir.

Bu sorunu çözmek için iş akışınızı Exchange Online gönderen [sınırlarını](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)aşmadan e-posta iletileri gönderecek şekilde yapılandırın. Örneğin, iş akışında bir duraklama kullanın, e-postayı bir Office 365 grubuna, dağıtım grubuna veya posta etkin güvenlik grubuna gönderin veya iletiyi aynı anda 200'den az alıcıya gönderin.


Daha fazla bilgi için aşağıdaki [makaleye](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)bakın.

## <a name="related-topics"></a>İlgili konular
- [Akış Oluştur](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ve Akış](https://flow.microsoft.com/blog/sharepoint-and-flow/) 