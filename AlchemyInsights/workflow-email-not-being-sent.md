---
title: İş akışı e-postası gönderilmiyor
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
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749029"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>SharePoint listesi veya kitaplığı için iş akışı e-postası gönderilmiyor

1. İş akışlarından gelen e-posta tüm kullanıcılara veya yalnızca belirli kullanıcılara gönderilmez veya **e-posta iletisinin gönderilemediği hatayı görürsünüz. e-postanın geçerli bir alıcısı olduğundan emin olun**.

    Kullanıcının söz konusu site koleksiyonu için **tüm insan** izinleri grubunda (Kullanıcı bilgileri listesi) bulunup bulunmadığını denetleyin.  Örnek doğrudan URL: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0

    - Kullanıcı yoksa, kullanıcının sayfada oturum açıldığından emin olun. 
    - Bu bir dış kullanıcıysanız, davetinin kabul edilmiş olduğundan emin olun.
    - Kullanıcı izinler grubunda varsa, e-posta adresinin doğru olduğundan emin olun.
    - Kullanıcıların e-posta adresi burada ayarlanmamışsa, bu kullanıcı hesabının SharePoint 'in Kullanıcı profillerinden bu site koleksiyonuna eşitlenmesini zorlayan bir örnek uyarı oluşturun.
 
2. İş akışlarından gelen e-posta, site koleksiyonu yöneticilerine gönderilir, ancak diğer kullanıcılara değil **http <span>:</span>//_vti_bin/Client.XVC.Sp.Utilities.Utility.SendEmail**.
 

    [Bir SharePoint grubuna e-posta gönderdiğinizde erişim engellendi](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)bölümüne bakın.

    Ayrıca, **sınırlı erişimli kullanıcı izni kilitleme modu** site koleksiyonu özelliğinin etkin olmadığını doğrulayın.


## <a name="related-topics"></a>İlgili konular
SharePoint Online 'da Microsoft akışını denemek mi istiyorsunuz?
- [Akış oluştur](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ve akış](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


