---
title: İş akışı e-postası gönderiliyor
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049393"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>İş akışı e-postası SharePoint listesi veya kitaplık için göndermiyor

1. İş akışlarından gelen e-postalar tüm kullanıcılara veya yalnızca belirli kullanıcılara gönderilmez veya **e-posta iletisinin gönderilemeyeceği hatayı görürsünüz. E-postanın geçerli bir alıcıya sahip olduğundan emin olun.**

    Kullanıcının bu site koleksiyonu için **Tüm Kişiler** izinler grubunda (kullanıcı bilgileri listesi) bulunun.  Örnek doğrudan URL:<tenant><sitename>https:// .sharepoint.com/sites/ /_layouts/15/people.aspx? ÜyelikGroupId=0

    - Kullanıcı yoksa, kullanıcının sayfada oturum açmış olduğundan emin olun. 
    - Harici bir kullanıcıysa, davetlerinin kabul edildiğinden emin olun.
    - Kullanıcı izinler grubunda varsa, e-posta adresinin doğru olduğundan emin olun.
    - Kullanıcıların e-posta adresi burada ayarlanmıyorsa, o kullanıcı için sharepoint kullanıcı profillerinden bu site koleksiyonuna kullanıcı hesabının eşitlanmasını zorlayan bir örnek uyarı oluşturun.
 
2. İş akışlarından gelen e-postalar site koleksiyonu yöneticilerine gönderilir, ancak diğer kullanıcılara gönderilmez ve **http forbidden to https hatasını görürsünüz: //URL/_vti_bin/client.xvc.sp.utility.utility.SendEmail <span></span>**.
 

    Bir [SharePoint grubuna e-posta gönderdiğinde Erişim Reddedildi'yi](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)görün.

    Ayrıca, Sınırlı **erişimli kullanıcı izni kilitleme modu** site koleksiyonu özelliğinin etkin olmadığını doğrulayın.


## <a name="related-topics"></a>İlgili konular
SharePoint Online'da Microsoft Flow'u denemek ister misiniz?
- [Akış Oluştur](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ve Akış](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


