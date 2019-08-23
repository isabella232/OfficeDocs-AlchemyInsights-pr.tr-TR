---
title: SharePoint veya OneDrive öğeler silinemiyor
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: b25e6d144dcefcfed4258e78ad5cfd4089ba7d1e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558673"
---
# <a name="unable-to-delete-items"></a>Öğeler silinemiyor

SharePoint öğelerini silme sorunlar yaşıyorsunuz?

- Her zaman öğeyi silmek veya öğeyi kaldırmak bir [site koleksiyonu yöneticisi](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) denemesinde bulunması için [uygun izinlere](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) sahip olduğunuzdan emin olun.

- Olmadığını bir [bekletme ilkesi](https://docs.microsoft.com/office365/securitycompliance/retention-policies) ayarı öğede emin olun.

- Öğeyi başka bir kullanıcı [kullanıma](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) değil emin olun.

- Son olarak, yöneticilerin geçeceğinizi öğeleri silme gibi karmaşık yönetimi eylemleri gerçekleştirmenize olanak sağlayan komutlar zorla PowerShell kitaplığını içeren [SharePoint desenleri ve yöntemler](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) kullanabilirsiniz.
- [PNP dosyasını kaldırın.](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP klasörünü kaldırma](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP liste öğesi Kaldır](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP listesini Kaldır](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP alan (sütun) Kaldır](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)