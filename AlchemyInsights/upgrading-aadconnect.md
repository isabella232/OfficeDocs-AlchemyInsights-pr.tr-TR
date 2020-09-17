---
title: 932 yükseltme
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806059"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD Connect 'i yükseltme

Varsayılan olarak, Azure AD Connect için otomatik yükseltme etkinleştirilir ve bu da en son sürümü çalıştırdığınızdan emin olmanıza yardımcı olur. Otomatik yükseltme ayarlarını doğrulamak için, Azure AD PowerShell 'de **Get-ADSyncAutoUpgrade** cmdlet 'ini kullanın. Cmdlet, aşağıdaki değerlerden birini döndürür:

- **Etkin**: otomatik yükseltme etkin.

- **Devre dışı**: otomatik yükseltme devre dışı.

- **Askıya alındı**: Sistem artık otomatik yükseltmeleri almaya uygun değil. Bu değeri yapılandıramazsınız; sistem tarafından ayarlanır.

Daha fazla bilgi [için bkz.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

Azure AD Connect 'in en son sürümünü indirmek için gidin [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
