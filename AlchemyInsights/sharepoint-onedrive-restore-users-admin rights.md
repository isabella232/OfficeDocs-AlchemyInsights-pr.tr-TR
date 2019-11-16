---
title: Sorun Giderme Access, İş siteleri için OneDrive'a gönderilen iletileri reddetti
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766731"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Sorun Giderme Access, İş siteleri için OneDrive'a gönderilen iletileri reddetti

Bu sorun en sık bir kullanıcı silindiğinde ve aynı kullanıcı anaadı (UPN) ile yeniden oluşturulduğunda oluşur. Yeni hesap farklı bir PUID (Passport Unique ID) değeri kullanılarak oluşturulur. Kullanıcı bir site koleksiyonuna veya OneDrive'ına erişmeye çalıştığında, kullanıcıyanlış PUID'ye sahiptir. İkinci bir senaryo, Etkin Dizin kuruluş birimi (OU) ile dizin eşitlemesi içerir. Kullanıcılar Zaten SharePoint oturum açmış ve daha sonra farklı bir OU taşınır ve SharePoint ile yeniden senkronize, onlar bu sorunla karşılaşabilirsiniz.

1. Bu sorunu gidermek için, özgün UPN'yi makaledeki adımlarla geri yüklemeniz gerekir, [Office 365'te bir kullanıcıyı geri yüklemelisiniz.](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)
2. Orijinal kullanıcıyı geri yükleyemiyorsanız, bu adımları kullanarak eski kullanıcıyı OneDrive sitesinden kaldırmanız gerekir, [Kullanıcı bilgi listesinden bir kullanıcıyı kaldırın.]() 
3. Bu işlem yapıldıktan sonra, kullanıcının [OneDrive'ı için yönetici ekle](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) adımlarını izleyerek kullanıcının OneDrive sitesinin yönetici haklarına sahip olduğunu doğrulayabilirsiniz

İzin düzeyleri hakkında daha fazla bilgi için, [sharepoint'teki izin düzeylerini anlama makalesine](https://docs.microsoft.com/sharepoint/understanding-permission-levels)bakın.
