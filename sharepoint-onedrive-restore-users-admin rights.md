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
ms.openlocfilehash: ae4d2c00be6387744bdc84e1d8a021530f80f8fa
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715231"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>SharePoint ve OneDrive için kullanıcılara erişim vermek

<p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Bu sorun, kullanıcı olduğunda ve aynı kullanıcı asıl adı ile (UPN) yeniden oluşturulması en sık oluşur. Yeni hesabı farklı bir PUID (Passport benzersiz kimliği) değeri kullanılarak oluşturulur. Kullanıcı bir site koleksiyonu veya kendi OneDrive erişmeye çalıştığında, kullanıcı yanlış bir PUID sahiptir. İkinci senaryo directory eşitlemesi, Active Directory kuruluş birimi (OU) ile ilgilidir. Bunlar, kullanıcıların zaten SharePoint için oturumu ve ardından farklı bir kuruluş birimine taşınan ve SharePoint ile resynced, bu sorunla karşılaşabilirsiniz.</span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Özgün UPN makaledeki adımları geri bu sorunu çözmek için <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">geri bir kullanıcı Office 365'te.</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Bu yapıldıktan sonra kullanıcının sahip yönetici hakları OneDrive sitesine adımları izleyerek doğrulayabilirsiniz <a href="https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">admin's eklemek için bir kullanıcının OneDrive.</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">İzin düzeyleri hakkında daha fazla bilgi için, bkz: <a href="https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels">SharePoint izin düzeylerini anlama.</a>&nbsp;</span></p>
