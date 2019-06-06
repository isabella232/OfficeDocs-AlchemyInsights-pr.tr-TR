---
title: SharePoint ve OneDrive için kullanıcılara erişim vermek
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9326932e93970edc96396a141c9b36b14e7b4d4d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736667"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>SharePoint ve OneDrive için kullanıcılara erişim vermek

Bu sorun, kullanıcı olduğunda ve aynı kullanıcı asıl adı ile (UPN) yeniden oluşturulması en sık oluşur. Yeni hesabı farklı bir PUID (Passport benzersiz kimliği) değeri kullanılarak oluşturulur. Kullanıcı bir site koleksiyonu veya kendi OneDrive erişmeye çalıştığında, kullanıcı yanlış bir PUID sahiptir. İkinci senaryo directory eşitlemesi, Active Directory kuruluş birimi (OU) ile ilgilidir. Bunlar, kullanıcıların zaten SharePoint için oturumu ve ardından farklı bir kuruluş birimine taşınan ve SharePoint ile resynced, bu sorunla karşılaşabilirsiniz.

Bu sorunu gidermek için makaledeki adımları,[bir kullanıcının Office 365'te geri](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide)ile özgün UPN kurtarmalısınız.

Bu yapıldıktan sonra kullanıcının yönetici hakları OneDrive sitesine [Ekle admin kullanıcı OneDrive için kullanıcının](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) aşağıdaki adımları izleyerek sahip doğrulayabilirsiniz

İzin düzeyleri hakkında daha fazla bilgi için [SharePoint izin düzeylerini anlama](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels)makalesine bakın.
