---
title: Erişim reddedildi iletilerinde sorun giderme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767683"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>SharePoint/OneDrive Yönetim merkezinde erişim reddedildi iletilerinde sorun giderme

SharePoint/OneDrive yönetim merkezine gözatmaya çalışırken erişim reddedildi iletisi alıyorsanız, lütfen [kullanıcıya lisans atadığınızdan](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)emin olun. Kullanıcının lisansı varsa, bunların yönetim merkezlerine erişebilen [bir yönetici rolü atadıklarını](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) da unutmayın.

Bu sorun, bir Kullanıcı silindiğinde ve aynı kullanıcı asıl adıyla (UPN) yeniden oluşturulduğunda da oluşabilir. Yeni hesap farklı bir PUıD (Passport benzersiz KIMLIĞI) değeri kullanılarak oluşturulur. Kullanıcı bir site koleksiyonuna veya OneDrive 'a erişmeyi denediğinde, kullanıcının yanlış PUıD 'si vardır. İkinci senaryo, Active Directory kuruluş birimi (OU) ile dizin eşitlemesi içerir. Kullanıcılar zaten SharePoint 'te oturumlarsa, başka bir kuruluş birimine taşınmış ve SharePoint ile yeniden eşitleniyor

Bu sorunu çözmek için, özgün UPN 'yi makaledeki adımlarla geri yüklemelisiniz, [Microsoft 365 'da bir kullanıcıyı geri yüklemelisiniz](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Not: OneDrive veya SharePoint Yönetim Merkezi daha önce erişimi olan birden çok kullanıcı için kullanılamıyorsa geçici bir hizmet sorunu olabilir.  [Hizmet durumu panosunu denetleyin](https://portal.office.com/adminportal/home#/servicehealth).


