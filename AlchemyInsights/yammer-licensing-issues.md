---
title: Yammer lisanslama sorunları
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657296"
---
# <a name="yammer-licensing-issues"></a>Yammer lisanslama sorunları

Tüm kullanıcıların Yammer Enterprise hizmetini kullanmak için lisansı olmalıdır, ancak varsayılan olarak Yammer kullanıcıların hizmete erişmek için bir lisansı olmasını gerektirmez. Yönetici ayarı Yammer lisansı olmayan Microsoft 365 kullanıcılarını engelleyecek şekilde değiştirdiğinde, Yammer Kurumsal lisansı atanmamış kullanıcılar Yammer hizmetine erişemez. Daha fazla bilgi için [Office 365 'Da Yammer kullanıcı lisanslarını yönetme](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) konusuna bakın 

Lisanslar kullanıcılardan kaldırıldığında, Yammer kutucuğu artık görüntülenmez ve diğer hizmetler özellikleri gizlemek için lisans kaldırma özelliğini kullanabilir. Diğer durumlarda Özellikler görünmeye devam edebilir ancak çalışmaya devam eder.  

**Lisans, Kullanıcı için güncelleştirilmez**  

Bazen kullanıcıya lisans atanır ancak Yammer 'a erişemez. Bir toplu lisans ataması yapılırken gecikmelerin oluşma olasılığı daha yüksektir. Sistem eşzamanlı olarak çalıştığı için, Yammer kullanıcıları Azure AD 'de lisanslar değiştiği sırayla güncelleştirilmeyebilir. Lisans eşitleme sorunlarını bildirmek için bir destek durumunu açmadan önce 24 saate kadar bekleyin.  

**Toplu lisans ataması**  

Lisanslar Yönetim Merkezi veya PowerShell betiği aracılığıyla atanabilir. Daha fazla bilgi için, Office 365 PowerShell ile [kullanıcılara lisans atama](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ve [Kullanıcı hesaplarına lisans atama](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)konusuna bakın. 

Microsoft desteği, kod oluşturmayla ilgili Yardım sağlamaz, ancak Yammer lisans atamasında belgeler kullanılabilir. Daha fazla bilgi için [Windows PowerShell kullanarak Yammer lisanslarını yönetme](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)konusuna bakın.