---
title: SharePoint veya OneDrive 'da öğeler silinemiyor
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
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019603"
---
# <a name="unable-to-delete-items"></a>Öğeler silinemiyor

- Bekletme ilkeleri bunun nedeni, bu soruna neden olan ilgili tutmayı devre dışı bırakmanız veya dışarıda bırakmanız gerekir. Bekletme ilkesi veya tutma kaldırıldıktan sonra, değişikliğin geçerlilik kazanması 24 saate kadar sürebilir. Öğede [bekletme ilkesi](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) ayarı olmadığından emin olun.

- Site depolama sınırını aşmış olabilir, [site kotasını](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) artırıp öğeyi silin.

- Öğenin başka bir kullanıcıya [teslim](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) kullanılmadığından emin olun.

- Son olarak, Yöneticiler, Stubborn öğelerini silmeye zorlama gibi karmaşık yönetim eylemlerini gerçekleştirmenize olanak sağlayan bir PowerShell komutları kitaplığı içeren [SharePoint modellerini ve uygulamalarını](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) kullanabilir.
- [PNP dosyasını kaldırma](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP klasörünü kaldırma](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP listesi öğesini kaldır](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP listesini kaldır](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP alanı (sütun) kaldırma](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)