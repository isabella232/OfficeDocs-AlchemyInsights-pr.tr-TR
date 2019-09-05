---
title: SharePoint sitesine grup ekleme
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750540"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>SharePoint Online'da bağlı siteler oluştururken veya gruplandırmada sorunlar

Grup bağlantılı bir site oluştururken veya yeniden oluştururken karşılaşılan birkaç yaygın sorun vardır.

 Bir grubu ve bağlı sitesini sildiyseniz ve aynı URL'ye sahip başka bir site oluşturmak istiyorsanız, önceki siteyi kalıcı olarak kaldırmanız gerekir.

Karşıdan yükleme [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Powershell ile başlamak hakkında daha fazla bilgi için [SharePoint Online Management Shell ile başlarken](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet kullanarak Siteyi Silinmiş Sitelerden kaldırın.

Grup bağlantılı bir site oluşturuyorsanız ve bir uyarı alıyorsanız, aynı takma ada sahip başka bir grup zaten var, [Yönetici Merkezi'nden Office 365'teki](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)varolan grupları denetleyin. Sorunu gidermek için, artık gerekli değilse varolan grubu silin veya farklı bir takma ad atanmış siteyi oluşturun.

SharePoint ile modern gruplar oluşturmanın ve kullanmanın farklı yolları vardır.

Varolan siteleri bir Office 365 grubuna bağlayabilirsiniz. Daha fazla bilgi için [bkz.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)

Office 365 grubuna bağlı bir site oluşturmak için bir Ekip Sitesi oluşturmanız gerekir. Daha fazla bilgi için bkz: [SharePoint'te bir ekip sitesi oluştur.](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)

