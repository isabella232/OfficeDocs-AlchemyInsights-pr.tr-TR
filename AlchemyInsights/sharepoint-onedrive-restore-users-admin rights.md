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
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511204"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Sorun Giderme Access, İş siteleri için OneDrive'a gönderilen iletileri reddetti

Bu sorun en sık bir kullanıcı silindiğinde ve aynı kullanıcı anaadı (UPN) ile yeniden oluşturulduğunda oluşur. Yeni hesap farklı bir PUID (Passport Unique ID) değeri kullanılarak oluşturulur. Kullanıcı bir site koleksiyonuna veya OneDrive'ına erişmeye çalıştığında, kullanıcıyanlış PUID'ye sahiptir. İkinci bir senaryo, Etkin Dizin kuruluş birimi (OU) ile dizin eşitlemesi içerir. Kullanıcılar Zaten SharePoint oturum açmış ve daha sonra farklı bir OU taşınır ve SharePoint ile yeniden senkronize, onlar bu sorunla karşılaşabilirsiniz.

1. Bu sorunu gidermek için, orijinal UPN'yi makaledeki adımları geri yüklemeniz gerekir, [Microsoft 365'teki bir kullanıcıyı geri yüklemelisiniz.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)
2. Orijinal kullanıcıyı geri yükleyemiyorsanız, bu adımları kullanarak eski kullanıcıyı OneDrive sitesinden kaldırmanız gerekir, [Kullanıcı bilgi listesinden bir kullanıcıyı kaldırın.]() 
3. Bu işlem yapıldıktan sonra, kullanıcının [OneDrive'ı için yönetici ekle](https://docs.microsoft.com/sharepoint/manage-user-profiles) adımlarını izleyerek kullanıcının OneDrive sitesinin yönetici haklarına sahip olduğunu doğrulayabilirsiniz

İzin düzeyleri hakkında daha fazla bilgi için, [sharepoint'teki izin düzeylerini anlama makalesine](https://docs.microsoft.com/sharepoint/understanding-permission-levels)bakın.
