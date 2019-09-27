---
title: Veri konumu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207281"
---
# <a name="data-location"></a>Veri konumu

Yönetici merkezinde veya PowerShell üzerinden Exchange Online'a bağlanarak Office 365 kiracınızın konumunu görüntüleyebilirsiniz.


**Yönetici merkezi:**
1. [Yönetici merkezine](https://admin.microsoft.com/Adminportal/Home)giriş yapın.
2. **Ayarlar** > **Organizasyonu profilini**seçin.
3. **Veri konumu**altında, **ayrıntıları görüntüle'yi**seçin.


**Powershell:**
1. Windows PowerShell'i kullanarak Exchange Online'a bağlanın.
2. Kiracınızın özelliklerinin listesini görüntülemek için [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet'i çalıştırın. 
3. OrganizationId özelliğine bakın.

EXO ve SPO için veri konumuna sahip olduğunuzda, [verilerinizin bulunduğu yerden](https://products.office.com/where-is-your-data-located)kullanabileceğiniz diğer hizmetlerin veri konumunu belirleyebilirsiniz.