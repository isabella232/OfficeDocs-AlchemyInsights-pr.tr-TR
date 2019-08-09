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
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270692"
---
# <a name="workflow-email-is-not-being-sent"></a>İş akışı e-posta gönderme

1. Tüm kullanıcıları veya yalnızca belirli kullanıcıların iş akışları gelen e-posta gönderilmez veya gördüğünüz hata **e-posta iletisi gönderilemez. Geçerli bir alıcı e-posta olup olmadığını**.

    Onay grubundaki **Tüm kişilerin** izinleri (kullanıcı bilgileri listesi) bu site koleksiyonu için varsa.  Örnek doğrudan URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Kullanıcı yoksa, kullanıcı sayfaya oturum emin olun. 
    - Harici kullanıcı ise, kendi daveti kabul ettiğinden emin olun.
    - Kullanıcı grubu izinleri yoksa e-posta adresinin doğru olduğundan emin olun.
    - Kullanıcıların e-posta adresi burada ayarlı değilse, daha sonra eşitleme, kullanıcı hesabının bu site koleksiyonu için olan kullanıcı profilleri SharePoint'ten zorlar, bu kullanıcı için bir örnek uyarıyı oluşturun.
 
2. E-postadan iş akışları site koleksiyonu yöneticileri, ancak diğer kullanıcılara gönderilen ve hata **HTTP Yasak için <spam> <spam> ** <spam> <spam>.
 

    [Gönderilen e-posta grupları, erişim engellendi](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups)bakın.

    Ayrıca, **sınırlı erişimli kullanıcı izni kilitleme modu** site koleksiyonu özelliği etkin olmadığından emin olun.


## <a name="related-topics"></a>İlgili konular
SharePoint çevrimiçi Microsoft Flow denemek istiyor?
- [Akış oluşturma](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ve akış](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


