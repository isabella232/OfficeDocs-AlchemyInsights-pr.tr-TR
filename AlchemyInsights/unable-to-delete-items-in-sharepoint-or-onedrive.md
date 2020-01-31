---
title: SharePoint veya OneDrive'daki öğeleri sileme
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571291"
---
# <a name="unable-to-delete-items"></a>Öğeleri sileme

Bekletme ilkeleri buna neden olabilir, bu soruna neden olan ilgili tutmayı devre dışı bırakmak veya hariç tutmanız gerekir. Bekletme ilkesi veya tutma kaldırıldıktan sonra, değişikliğin etkili olması 24 saat kadar sürebilir. Öğeüzerinde [bekletme ilkesi](https://docs.microsoft.com/office365/securitycompliance/retention-policies) kurulumu olmadığından emin olun.

Site depolama sınırını aşmış, [site kotasını](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) artırmış ve öğeyi silmiş olabilir.

Öğenin başka bir kullanıcıya [kullanıma alınmadığından](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) emin olun.

Son olarak, yöneticiler, inatçı öğeleri zorla silme gibi karmaşık yönetim eylemleri gerçekleştirmenize olanak tanıyan PowerShell komutlarının kitaplığını içeren [SharePoint Desenleri ve Uygulamaları](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) 'nı (PnP) kullanabilir.
- [PNP dosyayı kaldırma](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP Klasörünü Kaldırma](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP Liste Öğeyi Kaldırma](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP Listesini Kaldır](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP Alanını Kaldırma (Sütun)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)