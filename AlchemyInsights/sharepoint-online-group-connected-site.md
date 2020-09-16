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
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771228"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>SharePoint 'te grup bağlantılı sitesi oluştururken karşılaşılan sorunlar

1. Grup bağlantılı bir siteyi oluştururken veya yeniden oluştururken karşılaşılan bazı yaygın sorunlar oluştu.
Bir grubu ve bağlı siteyi sildiyseniz ve aynı URL 'ye sahip başka bir site oluşturmak istiyorsanız, önceki siteyi kalıcı olarak kaldırmanız gerekir.

   - [SPO Yönetim Kabuğu 'nu](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) indirin
   - PowerShell ile çalışmaya başlama hakkında daha fazla bilgi için [SharePoint Online Yönetim Kabuğu ile çalışmaya](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)başlama konusuna bakın.
   - [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell cmdlet 'Ini kullanarak siteyi silinmiş sitelerden kaldırın. Grup sitelerini kalıcı olarak silmek için PowerShell gereklidir.

1. Grup bağlantılı bir site oluşturuyorsanız ve bir uyarı alırsanız: **aynı diğer ada sahip başka bir grup zaten varsa**, [Microsoft 365 Yönetim merkezinden](https://admin.microsoft.com/AdminPortal/Home#/groups)var olan grupları işaretleyin. Sorunu çözmek için, artık gerekmiyorsa var olan grubu silin veya başka bir diğer adla atanmış olan siteyi silin.

1. SharePoint ile modern gruplar oluşturmanın ve kullanmanın farklı yolları vardır.

   - Var olan siteleri Microsoft 365 grubuna bağlayabilirsiniz. Daha fazla bilgi için [SharePoint kullanıcı arabirimini kullanarak Microsoft 365 grubunu bağlama](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)bölümüne bakın.
   - Microsoft 365 Group bağlantılı sitesi oluşturmak için [ekip sitesi](https://admin.microsoft.com/sharepoint)oluşturmanız gerekir.
