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
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 210f230929db72027a0f729b17901fe88eb45709
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757311"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="c3569-102">Yükseltme Azure AD bağlama</span><span class="sxs-lookup"><span data-stu-id="c3569-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="c3569-103">Varsayılan olarak, Otomatik yükseltme, sağlamaya yardımcı olan en son sürümünü çalıştırdığınızı Azure AD bağlantı için etkinleştirilir.</span><span class="sxs-lookup"><span data-stu-id="c3569-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="c3569-104">Otomatik yükseltme ayarlarını doğrulamak için Azure AD PowerShell içinde **Get-ADSyncAutoUpgrade** cmdlet'ini kullanın.</span><span class="sxs-lookup"><span data-stu-id="c3569-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="c3569-105">Cmdlet aşağıdaki değerlerden birini döndürür:</span><span class="sxs-lookup"><span data-stu-id="c3569-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="c3569-106">**Etkin**: Otomatik yükseltme etkindir.</span><span class="sxs-lookup"><span data-stu-id="c3569-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="c3569-107">**Devre dışı**: Otomatik yükseltme devre dışıdır.</span><span class="sxs-lookup"><span data-stu-id="c3569-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="c3569-108">**Beklemede**: sistem artık otomatik yükseltme almaya uygun değil.</span><span class="sxs-lookup"><span data-stu-id="c3569-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="c3569-109">Bu değer yapılandıramazsınız; Bu sistem tarafından ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="c3569-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="c3569-110">Daha fazla bilgi için bkz: [Otomatik yükseltme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="c3569-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="c3569-111">Azure AD Bağlan'ın en son sürümünü karşıdan yüklemek için şu adrese gidin [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="c3569-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
