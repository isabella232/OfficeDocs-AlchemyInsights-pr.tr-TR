---
title: Bir grup için bir SharePoint sitesi ekleme
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507867"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Çevrimiçi SharePoint siteleri oluşturma veya gruba bağlı sorunlar

Birkaç site veya bir grup oluşturarak yeniden bağlandığında karşılaşılan genel sorunlar vardır.

 Bir grup ve bağlantılı sitesi silmiş ve aynı URL ile başka bir site oluşturmak istiyorsanız, önceki site kalıcı olarak kaldırmak gerekir.

[SPO Yönetim Kabuğu'nu](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) indirin

 Powershell ile çalışmaya başlama hakkında daha fazla bilgi için bkz: [SharePoint çevrimiçi Yönetim Kabuğu ile Başlarken](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Siteyi [Kaldır-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet'ini kullanarak siteleri silinmiş kaldırmak.

Bir grup bağlanılan site oluşturuyorsanız ve aynı ada sahip başka bir grup zaten var olan bir uyarı alırsınız, varolan [Office 365 Yönetim Merkezi'nden](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)gruplarından denetleyin. Bu sorunu çözmek, artık gerekli değilse, varolan bir grubu silerseniz veya site ile farklı bir diğer ad oluşturmak için atanmış.

Oluşturmak ve SharePoint ile modern grupları kullanmak için farklı yolları vardır.

Bir Office 365 gruba varolan sitelere bağlanabilir. Daha fazla bilgi için bkz: [SharePoint kullanıcı ineterface kullanarak bir Office 365 Grup Bağlan](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Office 365 Grup bağlanılan site oluşturmak için bir ekip sitesi oluşturmanız gerekir. Daha fazla bilgi için bkz: [SharePoint ekip sitesinde oluşturma](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

