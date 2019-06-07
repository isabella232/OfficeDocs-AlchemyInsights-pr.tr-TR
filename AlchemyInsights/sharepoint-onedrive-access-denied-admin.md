---
title: Erişim reddedildi iletisi ile ilgili sorunları giderme
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760360"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Sharepoint/OneDrive Yönetim Merkezi erişim engellendi iletilerinde sorun giderme

Erişim engellendi iletisi Sharepoint/OneDrive yönetim merkezine gitmek çalışırken alıyorsanız, lütfen emin olun o [kullanıcı için bir lisans atayın](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Kullanıcı lisansı varsa, ayrıca Yönetim Merkezleri erişebileceği [bir yönetici rolü atanmış](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) olduklarından emin olmalısınız.

Bu sorun, kullanıcı olduğunda ve aynı kullanıcı asıl adı ile (UPN) yeniden oluşturulması da oluşabilir. Yeni hesabı farklı bir PUID (Passport benzersiz kimliği) değeri kullanılarak oluşturulur. Kullanıcı bir site koleksiyonu veya kendi OneDrive erişmeye çalıştığında, kullanıcı yanlış bir PUID sahiptir. İkinci senaryo directory eşitlemesi, Active Directory kuruluş birimi (OU) ile ilgilidir. Bunlar, kullanıcıların zaten SharePoint için oturumu ve ardından farklı bir kuruluş birimine taşınan ve SharePoint ile resynced, bu sorunla karşılaşabilirsiniz.

Bu sorunu gidermek için makaledeki adımları, [bir kullanıcının Office 365'te geri](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)ile özgün UPN kurtarmalısınız.

Not: bir OneDrive veya SharePoint Yönetim Merkezi önceden erişimi olduğu birden çok kullanıcı için kullanılabilir durumda değilse, bir geçici olarak hizmet sorunu olabilir.  [Hizmet durumu panoyu kontrol edin](https://portal.office.com/adminportal/home#/servicehealth).


