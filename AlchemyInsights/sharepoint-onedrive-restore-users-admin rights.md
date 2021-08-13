---
title: Sitelere erişim reddedildi iletileriyle ilgili OneDrive İş giderme
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957813"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Sitelere erişim reddedildi iletileriyle ilgili OneDrive İş giderme

Bu sorun en sık, kullanıcı silindiğinde ve aynı kullanıcı asıl adıyla (UPN) yeniden oluşturulduğunda ortaya çıkar. Yeni hesap, farklı bir PUID (Passport Benzersiz Kimliği) değeri kullanılarak oluşturulur. Kullanıcı site koleksiyonuna veya kendi kimlik bilgilerine erişmeyi OneDrive, kullanıcının yanlış PUID'si olur. İkinci senaryo, Bir Active Directory kuruluş birimiyle (OU) dizin eşitlemesi içerir. Kullanıcılar daha önce SharePoint'de oturum açmalı ve sonra başka bir OU'ya taşınmış ve SharePoint ile yeniden eşitlise, bu sorunla sınmış olabilir.

1. Bu sorunu çözmek için, İlk UPN'yi Şu [](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)makaledeki Adımlarla geri yüklelisiniz: Microsoft 365.
2. Özgün kullanıcıyı geri yükleye değilken, şu adımları kullanarak eski OneDrive kaldırmanız gerekir: Kullanıcı [bilgileri listesinden kullanıcı kaldırma](). 
3. Bu yapıldıktan sonra, Kullanıcının kullanıcı hesabı için yönetici ekleme OneDrive sitenin yönetici haklarına sahip olduğunu [doğru OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

İzin düzeyleri hakkında daha fazla bilgi için bu Makaledeki [izin düzeylerini anlama SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
