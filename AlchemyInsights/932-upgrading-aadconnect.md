---
title: 932 yükseltme AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9add88a0e4a2590639cbfc546afdcdf5e6aa4886
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28318206"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="35778-102">Yükseltme Azure AD bağlama</span><span class="sxs-lookup"><span data-stu-id="35778-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="35778-p101">Varsayılan olarak, Otomatik yükseltme, sağlamaya yardımcı olan en son sürümünü çalıştırdığınızı Azure AD bağlantı için etkinleştirilir. Otomatik yükseltme ayarlarını doğrulamak için Azure AD PowerShell içinde **Get-ADSyncAutoUpgrade** cmdlet'ini kullanın. Cmdlet aşağıdaki değerlerden birini döndürür:</span><span class="sxs-lookup"><span data-stu-id="35778-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="35778-106">**Etkin**: Otomatik yükseltme etkindir.</span><span class="sxs-lookup"><span data-stu-id="35778-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="35778-107">**Devre dışı**: Otomatik yükseltme devre dışıdır.</span><span class="sxs-lookup"><span data-stu-id="35778-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="35778-p102">**Beklemede**: sistem artık otomatik yükseltme almaya uygun değil. Bu değer yapılandıramazsınız; Bu sistem tarafından ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="35778-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="35778-110">Daha fazla bilgi için bkz: [Otomatik yükseltme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="35778-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="35778-111">Azure AD Bağlan'ın en son sürümünü karşıdan yüklemek için şu adrese gidin [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="35778-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

