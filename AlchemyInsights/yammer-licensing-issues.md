---
title: Yammer lisans sorunları
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148428"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="d7428-102">Yammer lisans sorunları</span><span class="sxs-lookup"><span data-stu-id="d7428-102">Yammer licensing issues</span></span>

<span data-ttu-id="d7428-103">Tüm kullanıcıların Yammer Enterprise hizmetini kullanmak için bir lisansa sahip olması gerekir, ancak varsayılan olarak Yammer kullanıcıların hizmete erişmek için bir lisansa sahip olmasını gerektirmez.</span><span class="sxs-lookup"><span data-stu-id="d7428-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="d7428-104">Bir yönetici, Yammer lisansı olmayan Microsoft 365 kullanıcılarını engellemek için ayarı değiştirdiğinde, Yammer Enterprise lisansı atanmayan kullanıcılar Yammer hizmetine erişemez.</span><span class="sxs-lookup"><span data-stu-id="d7428-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="d7428-105">Daha fazla bilgi için Bkz. [Office 365'teki Yammer kullanıcı lisanslarını yönet](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="d7428-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="d7428-106">Lisanslar kullanıcılardan kaldırıldığında, Yammer döşemesi artık görüntülenmez ve diğer hizmetler özellikleri gizlemek için lisans kaldırma özelliğini kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="d7428-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="d7428-107">Diğer durumlarda, özellikler hala görünebilir, ancak çalışması için lisans ataması gerektirir.</span><span class="sxs-lookup"><span data-stu-id="d7428-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="d7428-108">**Lisans kullanıcı için güncelleştirmiyor**</span><span class="sxs-lookup"><span data-stu-id="d7428-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="d7428-109">Bazen, bir kullanıcıya lisans atanır, ancak Hala Yammer'a erişemez.</span><span class="sxs-lookup"><span data-stu-id="d7428-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="d7428-110">Toplu lisans ataması devam ederken gecikmeler indaha olasıdır.</span><span class="sxs-lookup"><span data-stu-id="d7428-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="d7428-111">Yammer kullanıcıları, sistem eşeşitle çalıştığından, Azure AD'de lisanslar değiştirilince aynı sırada güncelleştirilemeyebilir.</span><span class="sxs-lookup"><span data-stu-id="d7428-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="d7428-112">Lisans eşitleme sorunlarını bildirmek için bir destek örneği açmadan önce 24 saat kadar bekleyin.</span><span class="sxs-lookup"><span data-stu-id="d7428-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="d7428-113">**Toplu lisans ataması**</span><span class="sxs-lookup"><span data-stu-id="d7428-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="d7428-114">Lisanslar yönetici merkezi veya PowerShell komut dosyası aracılığıyla atanabilir.</span><span class="sxs-lookup"><span data-stu-id="d7428-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="d7428-115">Daha fazla bilgi için, [kullanıcılara lisans atama](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ve [Office 365 PowerShell ile kullanıcı hesaplarına lisans atama](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)'ya bakın.</span><span class="sxs-lookup"><span data-stu-id="d7428-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="d7428-116">Microsoft Destek komut dosyası oluşturma konusunda yardım sağlamaz, ancak Yammer lisans atamasıyla ilgili belgeler kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="d7428-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="d7428-117">Daha fazla bilgi için [Windows PowerShell'i kullanarak Yammer lisanslarını yönet'e](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)bakın.</span><span class="sxs-lookup"><span data-stu-id="d7428-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>