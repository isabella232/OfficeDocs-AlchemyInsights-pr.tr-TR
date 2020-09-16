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
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731583"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Günlük e-posta sınırı aşıldı. İş akışı askıya alındı.

Bu hata aşağıdaki senaryolarda alabilirsiniz:

- SharePoint Online 'da SharePoint 2010 veya SharePoint 2013 Workflow Platform türünü kullanan bir iş akışınız var.
- İş akışı, tek seferde 10.000 ' ten 200 fazla kullanıcıya veya dakikada 30 iletiden uzun bir e-posta iletisi gönderecek şekilde yapılandırılmıştır.
- İş akışını çalıştırdığınızda, e-posta iletisi gönderilmez ve aşağıdaki davranışı fark edebilirsiniz:
    - SharePoint 2013 Platform türünü kullanan bir iş akışı için **Iş akışı durumu** sayfasına gidin. Iş akışı durumu sayfasında, **Iç durum** **başlatıldı**olarak ayarlanır ve bilgi balonunun **alıcıya gönderilememe**durumu görüntülenir.

Bu sorunu geçici olarak çözmek için, iş akışınızı, [Exchange Online gönderici sınırlarını](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)aşmadan e-posta iletilerini gönderecek şekilde yapılandırın. Örneğin, iş akışında Pause kullanın, e-postayı bir Microsoft 365 grubuna, bir dağıtım grubu veya posta etkin güvenlik grubuna gönderebilir veya iletiyi 200 'den daha az alıcıya gönderin.


Daha fazla bilgi için aşağıdaki [makaleye](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)bakın.

## <a name="related-topics"></a>İlgili konular
- [Akış oluştur](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ve akış](https://flow.microsoft.com/blog/sharepoint-and-flow/) 