---
title: Günlük e-posta sınırı aşıldı. İş akışı askıya alınır.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059658"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Günlük e-posta sınırı aştı. İş akışı askıya alınır.

Bu hata aşağıdaki senaryolarda alınan:

- Bir iş akışı SharePoint 2010 SharePoint veya SharePoint 2013 iş akışı platform türü kullanan çevrimiçi olarak vardır.
- İş akışı, bir saat, günde 10. 000'den fazla alıcı veya dakika başına 30'dan fazla ileti 200'den fazla kullanıcılara özel e-posta iletisi göndermek için yapılandırılır.
- İş akışı çalıştırdığınızda, e-posta iletisi gönderilmez ve aşağıdaki davranışla karşılaşırsınız:
    - SharePoint 2013 platform türünü kullanarak iş akışı, **İş akışı durumu** sayfasına gidin. İş akışı durumu sayfasında **İç durumu** **başlatıldı**olarak ayarlanır ve **alıcıya gönderilemiyor**bilgi balonu görüntüler.

Bu soruna geçici bir çözüm için [gönderen Exchange Online sınırları](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)aşmadan e-posta iletileri göndermek için iş akışı yapılandırın. Örneğin, iş akışında duraklama kullanmak, Office 365 grup, bir dağıtım grubu veya posta etkin güvenlik grubunun e-posta Gönder veya aynı anda 200'den daha az sayıda alıcıya göndermek.


Daha fazla bilgi için aşağıdaki [makaleye](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)bakın.

## <a name="related-topics"></a>İlgili konular
- [Akış oluşturma](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ve akış](https://flow.microsoft.com/blog/sharepoint-and-flow/) 