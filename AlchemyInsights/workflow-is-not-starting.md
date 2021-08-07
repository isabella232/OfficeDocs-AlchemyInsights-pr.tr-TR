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
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907758"
---
# <a name="workflow-is-not-starting"></a>İş akışı başlat değil

- SharePoint 2010 ve SharePoint 2013 iş akışları başlat değil.

    - İş akışınız başlatmüyorsa, kullanıcıların iş akışı ilerleme durumuyla ilgili aralıklı gecikmeler yaşamaları için geçici bir hizmet sorunu olabilir. Hizmet Durumu [Panosuna bakarak,](https://admin.microsoft.com/AdminPortal/Home/servicehealth) kuruma etki olup yardımcı olup denetlemeniz gerekir.

    - Bu sorunu ilk kez gördükten sonra 24 saati geçtiyse lütfen destek bileti kaydı yapın. Birçok durumda, zaten bir çözüm üzerinde çalışıyoruz. Lütfen bir çözümü tamamlamak için en az 24 saat bekleyin.

- SharePoint gecikmeli 2010 iş akışları.

    - Bu durum, iş akışı büyük gruplar içinde tetiklenirse ortaya çıkar. (örneğin, aynı anda birkaç öğe ekli olduğunda).

    - İş akışları gerçek zamanlı olarak çalıştıracak şekilde tasarlanmay, bu nedenle gecikme tasarım davranışıdır.

   -  İş Akışı karmaşık Genişletilebilir Nesne İşaretleme Dili (X İŞARETLEME Dili) ise, derleme işlemi yavaş olabilir. Bu [makaleyi](https://support.microsoft.com//kb/3043697) okuyun.

    - Microsoft SharePoint 2013 İş Akışı platform türünü kullanarak iş akışını basitleştirmeli veya yeniden tasarlamalı.

    - İş akışı geçmişinizin büyük büyümeleri varsa, öğeleri temizlemek veya yeni bir geçmiş listesi oluşturmak iyi olabilir.

        Daha Fazla Bilgi : [İş Akışı Geçmişini Temizleme](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>İlgili konular
SharePoint Online'Microsoft Flow denemek mi istiyor musunuz?
- [Yeni Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ve Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
