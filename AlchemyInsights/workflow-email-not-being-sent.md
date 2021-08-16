---
title: İş akışı e-postası göndern mi?
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072540"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>İş akışı e-postası bir liste veya SharePoint gönderilmez

1. İş akışlarından gelen e-postalar tüm kullanıcılara veya yalnızca belirli kullanıcılara gönderilmez ya da E-posta iletisi gönderile ilgili hatayı **görüyorsunuz. E-postanın** geçerli bir alıcısına sahip olduğundan emin olun.

    Kullanıcının, o site koleksiyonunun **Tüm Kişiler izinler** grubunda (kullanıcı bilgileri listesi) yer alıyor olup olmadığını denetleyin.  Örnek doğrudan URL: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Kullanıcı yoksa, sayfada oturum olduğundan emin olun. 
    - Dış kullanıcı ise, davetin kabul edildi olduğundan emin olun.
    - Kullanıcı izinler grubunda bulunuyorsa, e-posta adresinin doğru olduğundan emin olun.
    - Kullanıcıların e-posta adresi burada ayarlanmazsa, bu kullanıcı için, kullanıcının hesabını SharePoint'den bu site koleksiyonuna eşitlemeyi güçten örnek bir uyarı oluşturun.
 
2. İş akışlarından gelen e-posta site koleksiyonu yöneticilerine gönderilir, ancak diğer kullanıcılara gönderilmez **ve http Yasaklandı hatasınıhttps://url/_vti_bin/client.xvc.sp.utilities.utility.SendEmail <span></span>** adresine bakın.
 

    Bkz. SharePoint grubuna [e-posta SharePoint.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Ayrıca, Sınırlı **erişimli kullanıcı izni kilitleme modu** site koleksiyonu özelliğinin etkin olmadığını doğrulayın.


## <a name="related-topics"></a>İlgili konular
SharePoint Online'Microsoft Flow denemek mi istiyor musunuz?
- [Yeni Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ve Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


