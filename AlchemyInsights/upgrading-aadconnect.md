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
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="72af6-102">Azure AD Connect 'i yükseltme</span><span class="sxs-lookup"><span data-stu-id="72af6-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="72af6-103">Varsayılan olarak, Azure AD Connect için otomatik yükseltme etkinleştirilir ve bu da en son sürümü çalıştırdığınızdan emin olmanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="72af6-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="72af6-104">Otomatik yükseltme ayarlarını doğrulamak için, Azure AD PowerShell 'de **Get-ADSyncAutoUpgrade** cmdlet 'ini kullanın.</span><span class="sxs-lookup"><span data-stu-id="72af6-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="72af6-105">Cmdlet, aşağıdaki değerlerden birini döndürür:</span><span class="sxs-lookup"><span data-stu-id="72af6-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="72af6-106">**Etkin**: otomatik yükseltme etkin.</span><span class="sxs-lookup"><span data-stu-id="72af6-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="72af6-107">**Devre dışı**: otomatik yükseltme devre dışı.</span><span class="sxs-lookup"><span data-stu-id="72af6-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="72af6-108">**Askıya alındı**: Sistem artık otomatik yükseltmeleri almaya uygun değil.</span><span class="sxs-lookup"><span data-stu-id="72af6-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="72af6-109">Bu değeri yapılandıramazsınız; sistem tarafından ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="72af6-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="72af6-110">Daha fazla bilgi [için bkz.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)</span><span class="sxs-lookup"><span data-stu-id="72af6-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="72af6-111">Azure AD Connect 'in en son sürümünü indirmek için gidin [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="72af6-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
