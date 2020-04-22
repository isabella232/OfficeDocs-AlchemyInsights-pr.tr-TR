---
title: Sorun Giderme Access, İş siteleri için OneDrive'a gönderilen iletileri reddetti
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692821"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Sorun Giderme Access, İş siteleri için OneDrive'a gönderilen iletileri reddetti

Bu sorun en sık bir kullanıcı silindiğinde ve aynı kullanıcı anaadı (UPN) ile yeniden oluşturulduğunda oluşur. Yeni hesap farklı bir PUID (Passport Unique ID) değeri kullanılarak oluşturulur. Kullanıcı bir site koleksiyonuna veya OneDrive'ına erişmeye çalıştığında, kullanıcıyanlış PUID'ye sahiptir. İkinci bir senaryo, Etkin Dizin kuruluş birimi (OU) ile dizin eşitlemesi içerir. Kullanıcılar Zaten SharePoint oturum açmış ve daha sonra farklı bir OU taşınır ve SharePoint ile yeniden senkronize, onlar bu sorunla karşılaşabilirsiniz.

1. Bu sorunu gidermek için, orijinal UPN'yi makaledeki adımları geri yüklemeniz gerekir, [Microsoft 365'teki bir kullanıcıyı geri yüklemelisiniz.](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)
2. Orijinal kullanıcıyı geri yükleyemiyorsanız, bu adımları kullanarak eski kullanıcıyı OneDrive sitesinden kaldırmanız gerekir, [Kullanıcı bilgi listesinden bir kullanıcıyı kaldırın.]() 
3. Bu işlem yapıldıktan sonra, kullanıcının [OneDrive'ı için yönetici ekle](https://docs.microsoft.com/sharepoint/manage-user-profiles) adımlarını izleyerek kullanıcının OneDrive sitesinin yönetici haklarına sahip olduğunu doğrulayabilirsiniz

İzin düzeyleri hakkında daha fazla bilgi için, [sharepoint'teki izin düzeylerini anlama makalesine](https://docs.microsoft.com/sharepoint/understanding-permission-levels)bakın.
