---
title: 618 takvim paylaşım Ilkesi
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684250"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="fe74a-102">Takvim paylaşırken ilke hatası</span><span class="sxs-lookup"><span data-stu-id="fe74a-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="fe74a-103">Aşağıdakilerden birini yapın:</span><span class="sxs-lookup"><span data-stu-id="fe74a-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="fe74a-104">Uzak PowerShell 'i kullanarak Exchange Online 'a bağlanın.</span><span class="sxs-lookup"><span data-stu-id="fe74a-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="fe74a-105">Daha fazla bilgi için, [uzak PowerShell kullanarak Exchange Online 'A bağlanın](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="fe74a-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="fe74a-106">Şirket içi sunucuda Exchange Yönetim Kabuğu 'nu açın.</span><span class="sxs-lookup"><span data-stu-id="fe74a-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="fe74a-107">Kullanıcıya atanan paylaşım ilkesini belirleme.</span><span class="sxs-lookup"><span data-stu-id="fe74a-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="fe74a-108">Bunu yapmak için, aşağıdaki komutu çalıştırıp verilen ilkeye dikkat edin:</span><span class="sxs-lookup"><span data-stu-id="fe74a-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="fe74a-109">Kullanıcının paylaşım ilkesini güncelleyin.</span><span class="sxs-lookup"><span data-stu-id="fe74a-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="fe74a-110">Bunu yapmak için şu adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="fe74a-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="fe74a-111">Exchange Yönetim merkezini açın.</span><span class="sxs-lookup"><span data-stu-id="fe74a-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="fe74a-112">**Kuruluş**'a tıklayın ve ardından **bireysel paylaşım**altında kullanıcıya atanmış olan ilkeye çift tıklayın.</span><span class="sxs-lookup"><span data-stu-id="fe74a-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="fe74a-113">Bu, adım 2 ' de döndürülen ilkedir.</span><span class="sxs-lookup"><span data-stu-id="fe74a-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="fe74a-114">Paylaşım kuralı sayfasında, izin vermek istediğiniz takvim paylaşım düzeyini **paylaşmak istediğiniz bilgileri belirtip**seçin; **Kaydet**'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="fe74a-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="fe74a-115">Daha fazla bilgi için, [Kullanıcı takvimi paylaşmaya çalışıldığında "ilke bu düzeyde bir veya birden çok alıcıya izin vermeye izin vermiyor" hatasını](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)inceleyin.</span><span class="sxs-lookup"><span data-stu-id="fe74a-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
