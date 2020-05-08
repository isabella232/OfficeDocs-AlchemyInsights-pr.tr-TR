---
title: SharePoint sitesine grup ekleme
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: b54457427ffa563b6a6323d85e1c8800191eca11
ms.sourcegitcommit: d1aad215f8aa636ba89c93a13a0c9d90e997f752
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/06/2020
ms.locfileid: "44064413"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>SharePoint'te grup bağlantılı bir site oluştururken sorunlar

1. Grup bağlantılı bir site oluştururken veya yeniden oluştururken karşılaşılan bazı yaygın sorunlar.
Bir grubu ve bağlı sitesini sildiyseniz ve aynı URL'ye sahip başka bir site oluşturmak istiyorsanız, önceki siteyi kalıcı olarak kaldırmanız gerekir.

   - Karşıdan yükleme [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Powershell ile başlamak hakkında daha fazla bilgi için [SharePoint Online Management Shell ile başlarken](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)bakın.
   - [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet kullanarak Siteyi Silinmiş Sitelerden kaldırın. Powershell'in grup sitelerini kalıcı olarak silmesi gerekir.

1. Grup bağlantılı bir site oluşturuyorsanız ve bir uyarı alıyorsanız: **Aynı takma ada sahip başka bir grup zaten var,** [Microsoft 365 yönetici merkezinden](https://admin.microsoft.com/AdminPortal/Home#/groups)varolan grupları denetleyin. Sorunu gidermek için, artık gerekli değilse varolan grubu silin veya farklı bir takma ad atanmış siteyi oluşturun.

1. SharePoint ile modern gruplar oluşturmanın ve kullanmanın farklı yolları vardır.

   - Varolan siteleri bir Microsoft 365 grubuna bağlayabilirsiniz. Daha fazla bilgi için bkz: [SharePoint kullanıcı arabirimini kullanarak bir Microsoft 365 grubunu bağlayın.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Microsoft 365 grubuna bağlı bir site oluşturmak için bir [Ekip Sitesi](https://admin.microsoft.com/sharepoint)oluşturmanız gerekir.
