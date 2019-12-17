---
title: Erişim Reddedilen iletileri sorun giderme
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051445"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Sharepoint/OneDrive Yönetici Merkezi'nde Reddedilen iletilere Erişim Sorunu

Sharepoint/OneDrive Yönetici Merkezi'ne göz atlamaya çalışırken erişim reddedilen bir ileti alıyorsanız, lütfen [kullanıcıya bir lisans atadığınızdan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)emin olun. Kullanıcının bir lisansı varsa, yönetici merkezlerine erişebilecek [bir yönetici rolü](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) atanmış olduğundan da emin olmalısınız.

Bu sorun, bir kullanıcı silindiğinde ve aynı kullanıcı ana adı (UPN) ile yeniden oluşturulduğunda da oluşabilir. Yeni hesap farklı bir PUID (Passport Unique ID) değeri kullanılarak oluşturulur. Kullanıcı bir site koleksiyonuna veya OneDrive'ına erişmeye çalıştığında, kullanıcıyanlış PUID'ye sahiptir. İkinci bir senaryo, Etkin Dizin kuruluş birimi (OU) ile dizin eşitlemesi içerir. Kullanıcılar Zaten SharePoint oturum açmış ve daha sonra farklı bir OU taşınır ve SharePoint ile yeniden senkronize, onlar bu sorunla karşılaşabilirsiniz.

Bu sorunu gidermek için, özgün UPN'yi makaledeki adımlarla geri yüklemeniz gerekir, [Office 365'te bir kullanıcıyı geri yüklemeniz](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)gerekir.

Not: OneDrive veya SharePoint Yönetici merkezi daha önce erişimi olan birden çok kullanıcı tarafından kullanılamıyorsa, geçici bir hizmet sorunu olabilir.  [Hizmet durumu panosunu kontrol edin.](https://portal.office.com/adminportal/home#/servicehealth)


