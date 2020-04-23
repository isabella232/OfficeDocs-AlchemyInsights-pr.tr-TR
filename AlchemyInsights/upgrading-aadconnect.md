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
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="910ea-102">Azure AD Connect'i yükselt</span><span class="sxs-lookup"><span data-stu-id="910ea-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="910ea-103">Varsayılan olarak, Azure AD Connect için otomatik yükseltme etkinleştirilir ve bu da en son sürümü çalıştırdığınızdan emin olmaya yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="910ea-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="910ea-104">Otomatik yükseltme ayarlarını doğrulamak için Azure AD PowerShell'de **Get-ADSyncAutoUpgrade** cmdlet'ini kullanın.</span><span class="sxs-lookup"><span data-stu-id="910ea-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="910ea-105">Cmdlet aşağıdaki değerlerden birini döndürür:</span><span class="sxs-lookup"><span data-stu-id="910ea-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="910ea-106">**Etkin**: Otomatik yükseltme etkindir.</span><span class="sxs-lookup"><span data-stu-id="910ea-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="910ea-107">**Devre Dışı :** Otomatik yükseltme devre dışı bırakılır.</span><span class="sxs-lookup"><span data-stu-id="910ea-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="910ea-108">**Askıya :** Sistem artık otomatik yükseltme almaya uygun değildir.</span><span class="sxs-lookup"><span data-stu-id="910ea-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="910ea-109">Bu değeri yapılandıramazsınız; Sistem tarafından ayarlanmış.</span><span class="sxs-lookup"><span data-stu-id="910ea-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="910ea-110">Daha fazla bilgi için Otomatik [yükseltme'ye](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)bakın.</span><span class="sxs-lookup"><span data-stu-id="910ea-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="910ea-111">Azure AD Connect'in en son [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)sürümünü indirmek için ' e gidin.</span><span class="sxs-lookup"><span data-stu-id="910ea-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
