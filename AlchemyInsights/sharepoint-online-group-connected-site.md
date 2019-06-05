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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719501"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Bağlanılan site grubu SharePoint çevrimiçi oluşturun

<p><strong>Birkaç site veya bir grup oluşturarak yeniden bağlandığında karşılaşılan genel sorunlar vardır.&nbsp;</strong></p>  <p>1.Bir grup ve bağlantılı sitesi silmiş ve aynı URL ile başka bir site oluşturmak istiyorsanız, önceki site kalıcı olarak kaldırmak gerekir.</p>  <ul>  <li>Karşıdan <a title="SPO Yönetim Kabuğu" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO Yönetim Kabuğu</a> - powershell ile çalışmaya başlama hakkında daha fazla bilgi için bkz: <a title="SharePoint çevrimiçi Yönetim Kabuğu ile Başlarken" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">SharePoint çevrimiçi Yönetim Kabuğu ile Başlarken</a>. <br /><br /></li>  <li>Silinen siteleri kullanarak Site kaldırma <a title="SPODeletedSite Kaldır" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Kaldır-SPODeletedSite</a> powershell cmdlet.</li>  </ul>  <p>Bir grup bağlanılan site oluşturuyorsanız ve <strong>'zaten aynı ada sahip başka bir grup var'</strong>uyarı almak, varolan grupları denetleyin <a title="Yönetim Merkezi'nden Office 365" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 Yönetim Merkezi'nden</a>. Bu sorunu çözmek, artık gerekli değilse, varolan bir grubu silerseniz veya site ile farklı bir diğer ad oluşturmak için atanmış.&nbsp;</p>  <p><strong>Oluşturmak ve SharePoint ile modern grupları kullanmak için farklı yolları vardır.&nbsp;</strong></p>  <ol>  <li>Bir Office 365 gruba varolan sitelere bağlanabilir. Daha fazla bilgi için bkz: <a title="SharePoint kullanıcı ineterface kullanarak bir Office 365 Grup bağlanma" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">SharePoint kullanıcı ineterface kullanarak bir Office 365 Grup bağlanmak</a>.</li>  <li>Office 365 Grup bağlanılan site oluşturmak için bir ekip sitesi oluşturmanız gerekir. Daha fazla bilgi için bkz: <a title="içinde SharePoint ekip sitesi oluşturma" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">SharePoint'te ekip sitesi oluşturun.</a></li>  </ol>

