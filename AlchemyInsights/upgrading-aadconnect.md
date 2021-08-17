---
title: 932 AADConnect'i yükseltme
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
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104832"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD yükseltme Bağlan

Varsayılan olarak, en son sürümü çalıştırmanıza yardımcı Bağlan Azure AD Bağlan için otomatik yükseltme etkindir. Otomatik yükseltme ayarlarını doğrulamak için Azure AD PowerShell'de **Get-ADSyncAutoUpgrade** cmdlet'ini kullanın. Cmdlet, aşağıdaki değerlerden birini verir:

- **Etkin:** Otomatik yükseltme etkinleştirildi.

- **Devre Dışı:** Otomatik yükseltme devre dışı bırakıldı.

- **Askıya** alındı: Sistem artık otomatik yükseltme almaya uygun değil. Bu değeri yapılandıramazsanız; sistem tarafından ayarlanır.

Daha fazla bilgi için bkz. [Otomatik yükseltme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Azure AD Bağlan'nin en son sürümünü indirmek için, [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) gidin.
