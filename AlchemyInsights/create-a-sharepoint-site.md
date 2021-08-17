---
title: SharePoint oluşturma
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
ms.openlocfilehash: bf9380727fff415357884a5122e633f2254337d3db50e2b8656d94938f76d394
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080910"
---
# <a name="create-a-sharepoint-site"></a>SharePoint oluşturma

Site Yönetim Merkezi'nde [Etkin Sitelerden](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) site SharePoint yönetin. Daha fazla bilgi için [bkz. Yeni yönetim merkezinde SharePoint.](https://docs.microsoft.com/sharepoint/manage-site-creation) 

## <a name="tips"></a>İpuçları:

- Var **olan** sitenin URL'sini kullanarak site oluşturamazsanız. Bir siteyi sildikten sonra URL'yi yeniden kullanmak isterseniz, silinen sitenin hala Silinmiş siteler altında [yermiş olabilir.](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true) URL'yi yeniden kullanmak için sitenin kalıcı olarak silinmesi gerekir. Powershell ile bir siteyi tamamen kaldırmak için bkz. [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet örneği.
- Bazı kullanıcılar site oluşturamayabilecek. [Bkz. SharePoint Online'da site SharePoint yönetme.](https://docs.microsoft.com/sharepoint/manage-site-creation)
- Site, Beklenenden uzun oluşturma konusunda **takılmış** gibi görünüyor olabilir. Bu sorunu ilk kez gördükten sonra 24 saati geçtiyse lütfen destek bileti kaydı yapın. Birçok durumda, zaten bir çözüm üzerinde çalışıyoruz. Lütfen bir çözümü tamamlamak için en az 24 saat bekleyin.
