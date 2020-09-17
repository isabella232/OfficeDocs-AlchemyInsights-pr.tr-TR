---
title: SharePoint sitesi oluşturma
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806959"
---
# <a name="create-a-sharepoint-site"></a>SharePoint sitesi oluşturma

SharePoint Yönetim merkezinde [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) 'de site oluşturma veya yönetme. Daha fazla bilgi için [Yeni SharePoint Yönetim merkezinde siteleri yönetme](https://docs.microsoft.com/sharepoint/manage-site-creation)bölümüne bakın. 

## <a name="tips"></a>Ok

- Var olan bir sitenin URL 'sini içeren bir **site oluşturamazsınız.** Bir siteyi sildiyseniz ve URL 'YI yeniden kullanmayı düşünüyorsanız, silinen site yine [Silinmiş sitelerde](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)yer alabilir. URL 'YI yeniden kullanmak için sitenin kalıcı olarak silinmesi gerekir. Bir siteyi PowerShell ile tümüyle kaldırmak için [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet 'ine bakın.
- Bazı kullanıcılar site oluşturamaz. [SharePoint Online 'da site oluşturmayı yönetme konusuna bakın](https://docs.microsoft.com/sharepoint/manage-site-creation).
- Site **beklenenden uzun süre** içinde kalmış görünüyor. Bu sorunu ilk kez gördüğünüzde 24 saatten uzun bir süreyi geçmişse, lütfen bir destek bileti günlüğe yazılır. Birçok durumda bir çözüm üzerinde çalışıyoruz. Lütfen çözümü tamamlamak için en az 24 saat bekleyin.
