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
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707974"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>SharePoint/OneDrive Yönetim Merkezi'nde Erişim Reddedildi iletileriyle ilgili sorunları giderme

SharePoint/OneDrive Yönetim Merkezi'ne göz atamazken erişim reddedildi iletisi alıyorsanız, kullanıcıya lisans [atayın.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Kullanıcının lisansı varsa, bu kullanıcıya yönetim merkezlerine erişen bir [yönetici](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) rolü atanmalı.

Bu sorun, kullanıcı silindiğinde ve aynı kullanıcı asıl adıyla (UPN) yeniden oluşturulduğunda de oluşabilir. Yeni hesap, farklı bir PUID (Passport Benzersiz Kimlik) değeri kullanılarak oluşturulur. Kullanıcı bir site koleksiyonuna veya OneDrive'larına erişmeye çalıştığında, kullanıcının puid'i yanlış olur. İkinci senaryo, Active Directory kuruluş birimiyle (OU) dizin eşitlemesi içerir. Kullanıcılar daha önce SharePoint'te oturum açmışsa ve sonra başka bir OU'ya taşınmışsa ve SharePoint ile yeniden eşitlirse, bu sorunla sınmış olabilir.

Bu sorunu çözmek için, [microsoft 365'te](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)bir kullanıcıyı geri yükleme makalesinde verilen adımları kullanarak özgün UPN'yi geri yükleyebilirsiniz.

Not: OneDrive veya SharePoint Yönetim merkezi daha önce erişimi olan birden çok kullanıcı tarafından kullanılamıyorsa, geçici bir hizmet sorunu olabilir.  [Hizmet durumu panosuna göz ekleyin.](https://portal.office.com/adminportal/home#/servicehealth)


