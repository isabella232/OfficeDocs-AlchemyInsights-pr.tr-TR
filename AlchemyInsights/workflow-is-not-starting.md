---
title: İş akışı başlat değil
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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403763"
---
# <a name="workflow-is-not-starting"></a>İş akışı başlat değil

- SharePoint 2010 ve SharePoint 2013 iş akışları başlat değil.

    - İş akışınız başlatılmışsa, kullanıcıların iş akışı ilerleme durumuyla ilgili aralıklı olarak gecikmeler yaşamaları geçici bir hizmet sorunu olabilir. Hizmet Durumu [Panosuna bakarak,](https://admin.microsoft.com/AdminPortal/Home/servicehealth) kurumdan etkilenenin olup olduğunu kontrol edin.

    - Bu sorunu ilk kez gördükten sonra 24 saati geçtiyse lütfen destek bileti kaydı yapın. Birçok durumda, zaten bir çözüm üzerinde çalışıyoruz. Lütfen bize çözümü tamamlamak için en az 24 saat süre ver.

- SharePoint 2010 iş akışları gecikmeli olarak başlar.

    - İş akışı büyük toplu işlemlerde tetiklenirse bu durum ortaya çıkar. (örneğin, aynı anda birkaç öğe ekleniyorsa).

    - İş akışları gerçek zamanlı olarak çalıştıracak şekilde tasarlanmamalıdır, bu nedenle gecikme tasarım davranışıdır.

   -  İş Akışı Genişletilebilir Nesne İşaretleme Dili (XLANDı) karmaşıksa, derleme işlemi yavaş olabilir. Bu [makaleye](https://support.microsoft.com//kb/3043697) bakın.

    - İş akışını basitleştirmeli veya Microsoft SharePoint 2013 İş Akışı platform türünü kullanarak yeniden tasarlamalı.

    - İş akışı geçmişiniz büyüdüyse, öğeleri temizlemek veya yeni bir geçmiş listesi oluşturmak iyi olabilir.

        Daha Fazla Bilgi : [İş Akışı Geçmişini Temizleme](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>İlgili konular
SharePoint Online'da Microsoft Flow'u denemek mi istiyor musunuz?
- [Akış Oluşturma](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ve Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
