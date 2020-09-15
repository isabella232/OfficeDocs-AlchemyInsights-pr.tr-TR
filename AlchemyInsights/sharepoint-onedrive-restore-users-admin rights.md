---
title: OneDrive Iş sitelerine erişim reddedildi iletilerine sorun giderme
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670636"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>OneDrive Iş sitelerine erişim reddedildi iletilerine sorun giderme

Bu sorun en sık, Kullanıcı aynı Kullanıcı adı (UPN) ile silinip yeniden oluşturulduğunda oluşur. Yeni hesap farklı bir PUıD (Passport benzersiz KIMLIĞI) değeri kullanılarak oluşturulur. Kullanıcı bir site koleksiyonuna veya OneDrive 'a erişmeyi denediğinde, kullanıcının yanlış PUıD 'si vardır. İkinci senaryo, Active Directory kuruluş birimi (OU) ile dizin eşitlemesi içerir. Kullanıcılar zaten SharePoint 'te oturumlarsa, başka bir kuruluş birimine taşınmış ve SharePoint ile yeniden eşitleniyor

1. Bu sorunu çözmek için, [Microsoft 365 'da bir kullanıcıyı geri yüklemek](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)IÇIN özgün UPN 'yi makaledeki adımlarla geri yüklemelisiniz.
2. Özgün kullanıcıyı geri yükleyemezsiniz, bu adımları kullanarak eski kullanıcıyı OneDrive sitesinden kaldırmanız gerekir, Kullanıcı [bilgileri listesinden bir kullanıcıyı kaldırabilirsiniz](). 
3. Bu yapıldıktan sonra, kullanıcının [OneDrive sitesine yönetici ekleme](https://docs.microsoft.com/sharepoint/manage-user-profiles) adımlarını Izleyerek kullanıcının OneDrive sitesinde yönetici haklarına sahip olduğunu doğrulayabilirsiniz

İzin düzeyleri hakkında daha fazla bilgi için [SharePoint 'teki izin düzeylerini anlama](https://docs.microsoft.com/sharepoint/understanding-permission-levels)makalesine bakın.
