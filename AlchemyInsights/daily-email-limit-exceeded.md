---
title: Günlük e-posta sınırı aşıldı. İş akışı askıya alındı.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914671"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Günlük e-posta Sınırı Aşıldı. İş akışı askıya alındı.

Bu hata aşağıdaki senaryolarda alınmıştır:

- SharePoint Online'da SharePoint 2010 veya SharePoint iş akışı platform türünü kullanan bir iş akışınız var.
- İş akışı, bir defada 200'den fazla kullanıcıya özel e-posta iletisi, günde 10.000'den fazla alıcı veya dakikada 30'dan fazla ileti gönderecek şekilde yapılandırılır.
- İş akışını çalıştırsanız, e-posta iletisi gönderilmez ve aşağıdaki davranışı fark edebilirsiniz:
    - SharePoint 2013 platform türünü kullanan bir iş akışı için İş Akışı Durumu **sayfasına göz atabilirsiniz.** İş Akışı Durumu sayfasında, **İç Durum** başlatıldı olarak **ayarlanır ve** bilgi balonu Alıcıya **gönderemiyor .**

Bu soruna yardımcı olmak için, iş akışınızı gönderenin sınırlarını aşmadan [e-posta iletileri Exchange Online yapılandırabilirsiniz.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Örneğin, iş akışında biraz duraklama kullanın, e-postayı Microsoft 365 grubuna, dağıtım grubuna veya posta özelliği etkin bir güvenlik grubuna gönderin ya da iletiyi bir defada 200'den az alıcıya gönderin.


Daha fazla bilgi için aşağıdaki makaleye [bakın.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>İlgili konular
- [Yeni Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ve Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 