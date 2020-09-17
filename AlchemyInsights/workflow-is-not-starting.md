---
title: İş akışı başlamıyor
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
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794787"
---
# <a name="workflow-is-not-starting"></a>İş akışı başlamıyor

- SharePoint 2010 ve SharePoint 2013 iş akışları başlamıyor.

    - İş akışınız başlatılamıyorsa, kullanıcıların iş akışı ilerlemesiyle aralıklı gecikmelere neden olabileceği geçici bir hizmet sorunu olabilir. Kuruluşunuzun [etkilenmediklerini görmek Için hizmet durumu panosunu](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) denetleyin.

    - Bu sorunu ilk kez gördüğünüzde 24 saatten uzun bir süreyi geçmişse, lütfen bir destek bileti günlüğe yazılır. Birçok durumda bir çözüm üzerinde çalışıyoruz. Lütfen çözümü tamamlamak için en az 24 saat bekleyin.

- SharePoint 2010 iş akışları başlangıçta gecikti.

    - Bu, iş akışı büyük toplu işlerle tetiklendiğinde gerçekleşir. (örneğin, bir kerede birkaç öğe eklendiğinde).

    - İş akışları gerçek zamanlı çalışacak şekilde tasarlanmamıştır, böylece bir gecikme tasarım davranışıdır.

   -  Iş akışı karmaşık genişletilebilir nesne Işaretleme dili (XMOL) ise, derleme yavaş olabilir. [Bu](https://support.microsoft.com//kb/3043697) makaleyi denetleyin.

    - Microsoft SharePoint 2013 Iş akışı Platform türünü kullanarak iş akışını basitleştirin veya yeniden tasarlamanız gerekir.

    - İş akışı geçmişiniz büyürse, öğeleri temizlemek veya yeni bir geçmiş listesi oluşturmak isteyebilirsiniz.

        Daha fazla bilgi: [Iş akışı geçmişini temizle](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>İlgili konular
SharePoint Online 'da Microsoft akışını denemek mi istiyorsunuz?
- [Akış oluştur](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ve akış](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


