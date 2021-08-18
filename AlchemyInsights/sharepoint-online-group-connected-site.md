---
title: SharePoint sitesine grup ekleme
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318144"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>İş yerinde grup bağlantılı site oluştururken sık karşılaşılan SharePoint

1. Grubu ve bağlantılı sitesini sildikten sonra aynı URL'ye sahip başka bir site oluşturmak isterseniz, önceki siteyi kalıcı olarak kaldırmanız gerekir.

   - [SPO Yönetim Kabuğu'nu indirme](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Powershell'i ile çalışmaya başlama hakkında daha fazla bilgi için [bkz. çevrimiçi yönetim SharePoint başlama](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet'ini kullanarak Siteyi Silinmiş Sitelerden Kaldır. Grup sitelerini kalıcı olarak silmek için Powershell gereklidir.

1. Gruba bağlı bir site oluşturuyorsanız ve bir uyarı alırsanız: Aynı diğer adı olan başka bir grup zaten var, gruptan var olan [Microsoft 365 yönetim merkezi.](https://admin.microsoft.com/AdminPortal/Home#/groups) Sorunu çözmek için artık gerek kalmadı ise var olan grubu silin veya siteyi farklı bir diğer ad atanmış olarak oluşturun.

1. Yeni gruplarla modern grupları oluşturmanın ve kullanmanın farklı SharePoint.

   - Var olan siteleri bir grup çalışma Microsoft 365 babilirsiniz. Daha fazla bilgi için [bkz. Bağlan arabirimini Microsoft 365 bir SharePoint grubu kullanma](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Grup bağlantılı Microsoft 365 oluşturmak için Ekip Sitesi oluşturmanız [gerekir.](https://admin.microsoft.com/sharepoint)
