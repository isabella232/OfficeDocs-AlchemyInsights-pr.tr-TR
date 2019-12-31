---
title: Ortak yönetim
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: fe7dcebf847fbd7d91632e93e2253bf62ac659aa
ms.sourcegitcommit: 4ed431b2e1aed26d07bd7eba282531537d29ad0e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/30/2019
ms.locfileid: "40910486"
---
# <a name="co-management"></a><span data-ttu-id="69194-102">Ortak yönetim</span><span class="sxs-lookup"><span data-stu-id="69194-102">Co-management</span></span>

<span data-ttu-id="69194-103">**Config Manager Hybrid'den Intune'a geçiş için ön koşullar**</span><span class="sxs-lookup"><span data-stu-id="69194-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="69194-104">Bu makaleyi gözden [geçirin.](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa)</span><span class="sxs-lookup"><span data-stu-id="69194-104">Review [this article](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span></span>
- <span data-ttu-id="69194-105">[Kullanıcılarınıza Bir Intune lisansı ekleyin.](https://docs.microsoft.com/intune/licenses-assign)</span><span class="sxs-lookup"><span data-stu-id="69194-105">[Add an Intune license to your users](https://docs.microsoft.com/intune/licenses-assign).</span></span>
- <span data-ttu-id="69194-106">Co-management'ı yapılandırırken [Edge tarayıcısını](https://www.microsoft.com/windows/microsoft-edge) kullanın.</span><span class="sxs-lookup"><span data-stu-id="69194-106">Use the [Edge browser](https://www.microsoft.com/windows/microsoft-edge) when configuring Co-management.</span></span>

<span data-ttu-id="69194-107">**Config Manager istemcisini Intune tarafından yönetilen cihazlara nasıl yükleyebilirim?**</span><span class="sxs-lookup"><span data-stu-id="69194-107">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="69194-108">Bkz. [Intune MDM tarafından yönetilen Windows aygıtları.](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm)</span><span class="sxs-lookup"><span data-stu-id="69194-108">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="69194-109">**MdM yetkisini değiştirmek istersem ne olur?**</span><span class="sxs-lookup"><span data-stu-id="69194-109">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="69194-110">MDM Yetkilisi bir destek talebi açılmadan değiştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="69194-110">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="69194-111">MDM yetkinizi değiştirmenize yardımcı olmak için lütfen aşağıdaki belgeleri gözden geçirin:</span><span class="sxs-lookup"><span data-stu-id="69194-111">Please review the following documentation to assist in changing your MDM authority:</span></span>
- [<span data-ttu-id="69194-112">MDM Yetkisini Config Manager'dan Intune bağımsız olarak değiştirin</span><span class="sxs-lookup"><span data-stu-id="69194-112">Change MDM Authority from Config Manager to Intune standalone</span></span>](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-change-mdm-authority)
- [<span data-ttu-id="69194-113">MDM Yetkisini Intune tek başına Config Manager'a değiştirme</span><span class="sxs-lookup"><span data-stu-id="69194-113">Change MDM Authority from Intune standalone to Config Manager</span></span>](https://docs.microsoft.com/intune-classic/deploy-use/prerequisites-for-enrollment#what-to-do-if-you-choose-the-wrong-mdm-authority-setting)