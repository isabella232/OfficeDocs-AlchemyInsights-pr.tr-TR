---
title: 932 AADConnect Yükseltme
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766513"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD Connect'i yükselt

Varsayılan olarak, Azure AD Connect için otomatik yükseltme etkinleştirilir ve bu da en son sürümü çalıştırdığınızdan emin olmaya yardımcı olur. Otomatik yükseltme ayarlarını doğrulamak için Azure AD PowerShell'de **Get-ADSyncAutoUpgrade** cmdlet'ini kullanın. Cmdlet aşağıdaki değerlerden birini döndürür:

- **Etkin**: Otomatik yükseltme etkindir.

- **Devre Dışı :** Otomatik yükseltme devre dışı bırakılır.

- **Askıya :** Sistem artık otomatik yükseltme almaya uygun değildir. Bu değeri yapılandıramazsınız; Sistem tarafından ayarlanmış.

Daha fazla bilgi için Otomatik [yükseltme'ye](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)bakın.

Azure AD Connect'in en son [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)sürümünü indirmek için ' e gidin.
