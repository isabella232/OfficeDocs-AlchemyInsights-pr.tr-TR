---
title: 932 yükseltme AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: ff3f74348599788edd8ce0991fe49bb6a54b55af
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506103"
---
# <a name="upgrade-azure-ad-connect"></a>Yükseltme Azure AD bağlama

Varsayılan olarak, Otomatik yükseltme, sağlamaya yardımcı olan en son sürümünü çalıştırdığınızı Azure AD bağlantı için etkinleştirilir. Otomatik yükseltme ayarlarını doğrulamak için Azure AD PowerShell içinde **Get-ADSyncAutoUpgrade** cmdlet'ini kullanın. Cmdlet aşağıdaki değerlerden birini döndürür:

- **Etkin**: Otomatik yükseltme etkindir.

- **Devre dışı**: Otomatik yükseltme devre dışıdır.

- **Beklemede**: sistem artık otomatik yükseltme almaya uygun değil. Bu değer yapılandıramazsınız; Bu sistem tarafından ayarlanır.

Daha fazla bilgi için bkz: [Otomatik yükseltme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Azure AD Bağlan'ın en son sürümünü karşıdan yüklemek için şu adrese gidin [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
