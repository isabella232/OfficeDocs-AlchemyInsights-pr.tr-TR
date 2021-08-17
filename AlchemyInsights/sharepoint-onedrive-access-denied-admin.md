---
title: Erişim Reddedildi ileti sorunlarını giderme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085248"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>SharePoint/OneDrive Yönetim Merkezi'nde Erişim Reddedildi iletileriyle ilgili sorunları giderme

SharePoint/OneDrive Yönetim Merkezi'ne göz atarak göz atarak erişim reddedildi iletisi alıyorsanız, kullanıcıya lisans [atamayı unutmayın.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Kullanıcının lisansı varsa, bu kullanıcıya yönetim merkezlerine erişen bir [yönetici](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) rolü atanmalarına da izin ve erişiminizin olduğundan emin olun.

Bu sorun, kullanıcı silindiğinde ve aynı kullanıcı asıl adıyla (UPN) yeniden oluşturulduğunda de oluşabilir. Yeni hesap, farklı bir PUID (Passport Benzersiz Kimliği) değeri kullanılarak oluşturulur. Kullanıcı site koleksiyonuna veya kendi kimlik bilgilerine erişmeyi OneDrive, kullanıcının yanlış PUID'si olur. İkinci senaryo, Bir Active Directory kuruluş birimiyle (OU) dizin eşitlemesi içerir. Kullanıcılar daha önce SharePoint'de oturum açmalı ve sonra başka bir OU'ya taşınmış ve SharePoint ile yeniden eşitlise, bu sorunla sınmış olabilir.

Bu sorunu çözmek için, İlk UPN'yi Geri Yükleme makalesinde verilen Adımlarla [Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Not: Erişim OneDrive veya SharePoint Yönetim merkezi kullanılamıyorsa, geçici bir hizmet sorunu olabilir.  [Hizmet durumu panosuna göz ayın.](https://portal.office.com/adminportal/home#/servicehealth)


