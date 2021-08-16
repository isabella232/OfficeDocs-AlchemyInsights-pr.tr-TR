---
title: SharePoint veya OneDrive'de öğeler SharePoint silinemiyor
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038537"
---
# <a name="unable-to-delete-items"></a>Öğeler silinemiyor

- Bekletme ilkeleri buna neden olabilir, bu soruna neden olan ilgili saklamayı devre dışı bırakmanız veya dışarıda bırakmanız gerekir. Bekletme ilkesi veya saklama kaldırıldıktan sonra, değişikliğin etkili bir şekilde kaldırılması 24 saate kadar sürebilir. Öğede bekletme ilkesi [kurulumu olmadığının](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) garantiye sahip olduğundan emin olmak.

- Site depolama sınırını aşmış, site kotasını [artırmış ve](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) öğeyi silebilir.

- Öğenin başka bir [kullanıcıya kullanıma alınmış olduğundan](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) emin olun.

- Son olarak, yöneticiler SharePoint öğeleri silerek zorlar gibi karmaşık yönetim eylemleri gerçekleştirmenizi sağlayan PowerShell komutlarının kitaplığını içeren SharePoint Desenleri ve Uygulamaları [](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) kullanabilir.
- [PNP Dosyasını Kaldır](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP Klasörünü Kaldır](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP Liste Öğesini Kaldır](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP Listesini Kaldırma](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP Alanını Kaldırma (Sütun)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)