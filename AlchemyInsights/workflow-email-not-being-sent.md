---
title: İş akışı e-posta gönderme
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
- "1586"
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530911"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>İş akışı e-posta bir SharePoint listesi veya kitaplığı için gönderiliyor.

1. Tüm kullanıcıları veya yalnızca belirli kullanıcıların iş akışları gelen e-posta gönderilmez veya gördüğünüz hata **e-posta iletisi gönderilemez. Geçerli bir alıcı e-posta olup olmadığını**.

    Onay grubundaki **Tüm kişilerin** izinleri (kullanıcı bilgileri listesi) bu site koleksiyonu için varsa.  Örnek doğrudan URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Kullanıcı yoksa, kullanıcı sayfaya oturum emin olun. 
    - Harici kullanıcı ise, kendi daveti kabul ettiğinden emin olun.
    - Kullanıcı grubu izinleri yoksa e-posta adresinin doğru olduğundan emin olun.
    - Kullanıcıların e-posta adresi burada ayarlı değilse, daha sonra eşitleme, kullanıcı hesabının bu site koleksiyonu için olan kullanıcı profilleri SharePoint'ten zorlar, bu kullanıcı için bir örnek uyarıyı oluşturun.
 
2. E-postadan iş akışları site koleksiyonu yöneticileri, ancak diğer kullanıcılara gönderilen ve hata **için HTTP Yasak <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    [SharePoint grubuna bir e-posta gönderdiğinizde, erişim engellendi](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)bakın.

    Ayrıca, **sınırlı erişimli kullanıcı izni kilitleme modu** site koleksiyonu özelliği etkin olmadığından emin olun.


## <a name="related-topics"></a>İlgili konular
SharePoint çevrimiçi Microsoft Flow denemek istiyor?
- [Akış oluşturma](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ve akış](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


