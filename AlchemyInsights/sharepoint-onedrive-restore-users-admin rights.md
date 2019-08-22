---
title: İletiler için OneDrive iş siteleri için reddedildi erişim sorunlarını giderme
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 39f9b9b1ca22f6e5959e2b431fb373b0002c0a92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507831"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>İletiler için OneDrive iş siteleri için reddedildi erişim sorunlarını giderme

Bu sorun, kullanıcı olduğunda ve aynı kullanıcı asıl adı ile (UPN) yeniden oluşturulması en sık oluşur. Yeni hesabı farklı bir PUID (Passport benzersiz kimliği) değeri kullanılarak oluşturulur. Kullanıcı bir site koleksiyonu veya kendi OneDrive erişmeye çalıştığında, kullanıcı yanlış bir PUID sahiptir. İkinci senaryo directory eşitlemesi, Active Directory kuruluş birimi (OU) ile ilgilidir. Bunlar, kullanıcıların zaten SharePoint için oturumu ve ardından farklı bir kuruluş birimine taşınan ve SharePoint ile resynced, bu sorunla karşılaşabilirsiniz.

1. Bu sorunu gidermek için makaledeki adımları,[bir kullanıcının Office 365'te geri](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)ile özgün UPN kurtarmalısınız.
2. Özgün kullanıcı geri yükleyemezseniz, aşağıdaki adımları, [kullanıcı bilgileri listesinde bir kullanıcıyı kaldırmak]()kullanarak OneDrive sitesinden eski kullanıcı kaldırmanız gerekir. 
3. Bu yapıldıktan sonra kullanıcının yönetici hakları OneDrive sitesine [Ekle admin kullanıcı OneDrive için kullanıcının](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) aşağıdaki adımları izleyerek sahip doğrulayabilirsiniz

İzin düzeyleri hakkında daha fazla bilgi için [SharePoint izin düzeylerini anlama](https://docs.microsoft.com/sharepoint/understanding-permission-levels)makalesine bakın.
