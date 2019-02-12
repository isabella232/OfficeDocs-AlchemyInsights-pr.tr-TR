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
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="a2c7a-102">Yükseltme Azure AD bağlama</span><span class="sxs-lookup"><span data-stu-id="a2c7a-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="a2c7a-p101">Varsayılan olarak, Otomatik yükseltme, sağlamaya yardımcı olan en son sürümünü çalıştırdığınızı Azure AD bağlantı için etkinleştirilir. Otomatik yükseltme ayarlarını doğrulamak için Azure AD PowerShell içinde **Get-ADSyncAutoUpgrade** cmdlet'ini kullanın. Cmdlet aşağıdaki değerlerden birini döndürür:</span><span class="sxs-lookup"><span data-stu-id="a2c7a-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="a2c7a-106">**Etkin**: Otomatik yükseltme etkindir.</span><span class="sxs-lookup"><span data-stu-id="a2c7a-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="a2c7a-107">**Devre dışı**: Otomatik yükseltme devre dışıdır.</span><span class="sxs-lookup"><span data-stu-id="a2c7a-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="a2c7a-p102">**Beklemede**: sistem artık otomatik yükseltme almaya uygun değil. Bu değer yapılandıramazsınız; Bu sistem tarafından ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="a2c7a-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="a2c7a-110">Daha fazla bilgi için bkz: [Otomatik yükseltme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="a2c7a-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="a2c7a-111">Azure AD Bağlan'ın en son sürümünü karşıdan yüklemek için şu adrese gidin [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="a2c7a-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

