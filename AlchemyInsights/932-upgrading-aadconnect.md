---
title: 932 yükseltme AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8038d5ef768d6ee228db7d038ad71d926f4047f3
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29937964"
---
# <a name="upgrade-azure-ad-connect"></a>Yükseltme Azure AD bağlama

Varsayılan olarak, Otomatik yükseltme, sağlamaya yardımcı olan en son sürümünü çalıştırdığınızı Azure AD bağlantı için etkinleştirilir. Otomatik yükseltme ayarlarını doğrulamak için Azure AD PowerShell içinde **Get-ADSyncAutoUpgrade** cmdlet'ini kullanın. Cmdlet aşağıdaki değerlerden birini döndürür: 
  
- **Etkin**: Otomatik yükseltme etkindir. 
    
- **Devre dışı**: Otomatik yükseltme devre dışıdır. 
    
- **Beklemede**: sistem artık otomatik yükseltme almaya uygun değil. Bu değer yapılandıramazsınız; Bu sistem tarafından ayarlanır. 
    
Daha fazla bilgi için bkz: [Otomatik yükseltme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).
  
Azure AD Bağlan'ın en son sürümünü karşıdan yüklemek için şu adrese gidin [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
  

