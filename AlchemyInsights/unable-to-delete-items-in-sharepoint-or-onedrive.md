---
title: SharePoint veya OneDrive öğeler silinemiyor
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057792"
---
# <a name="unable-to-delete-items"></a>Öğeler silinemiyor

Öğeleri silme sorunlar yaşıyorsunuz?

- Her zaman öğeyi silmek veya öğeyi kaldırmak bir [site koleksiyonu yöneticisi](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) denemesinde bulunması için [uygun izinlere](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) sahip olduğunuzdan emin olun.

- Olmadığını bir [bekletme ilkesi](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) ayarı öğede emin olun.

- Öğeyi başka bir kullanıcı [kullanıma](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) değil emin olun.

- Son olarak, yöneticilerin geçeceğinizi öğeleri silme gibi karmaşık yönetimi eylemleri gerçekleştirmenize olanak sağlayan komutlar zorla PowerShell kitaplığını içeren [SharePoint desenleri ve yöntemler](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) kullanabilirsiniz. 
- [PNP dosyasını kaldırın.](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP klasörünü kaldırma](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP liste öğesi Kaldır](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP listesini Kaldır](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP alan (sütun) Kaldır](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)