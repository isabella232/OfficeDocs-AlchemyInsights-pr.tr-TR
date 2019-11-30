---
title: İlke ayarlarını karşılama
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627594"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="eb3df-102">Microsoft Teams'de toplantı ilkelerini yönetme</span><span class="sxs-lookup"><span data-stu-id="eb3df-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="eb3df-103">Toplantı ilkeleri, kuruluşunuzdaki kullanıcılar tarafından zamanlanan toplantılar için toplantı katılımcıları için kullanılabilen özellikleri denetlemek için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="eb3df-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="eb3df-104">Toplantı ilkelerinin bazı özellikleri henüz Takımlar yönetici merkezinde uygulanmayabilir (bunlar belgelerde "yakında" olarak etiketlenir).</span><span class="sxs-lookup"><span data-stu-id="eb3df-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="eb3df-105">Bu durumda veya Microsoft Teams yönetici merkezinde "İlkeyi şu anda güncelleştiremeyiz, ancak daha sonra tekrar deneyin" gibi bir hata alıyorsanız, Ekipler toplantı ilkeleri oluşturmak veya değiştirmek için PowerShell'i kullanmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="eb3df-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="eb3df-106">Toplantı ilkeleri hakkında daha fazla bilgi için aşağıdaki kaynaklara bakın:</span><span class="sxs-lookup"><span data-stu-id="eb3df-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="eb3df-107">İlkeler oluşturma, değişiklik yapma ve kullanıcıları ilkeye atama hakkında bilgi edinmek için [Bkz. Ekipler'deki toplantı ilkelerini yönet.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="eb3df-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="eb3df-108">PowerShell cmdlets kullanarak politika değişiklikleri yapmak için [Bkz. Teams PowerShell Genel Bakış.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="eb3df-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="eb3df-109">Ekipler toplantı ilkeleri için [Skype for Business PowerShell modüllerini](https://www.microsoft.com/download/details.aspx?id=39366) kullanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="eb3df-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="eb3df-110">Daha fazla bilgi için [\*-CsTeamsMeetingPolicy cmdlets belgelerini](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) inceleyin.</span><span class="sxs-lookup"><span data-stu-id="eb3df-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="eb3df-111">**Not:** İlke değişikliklerinin kullanıcılar için geçerli olması 24 saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="eb3df-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="eb3df-112">Yeni oluşturulan ilkelerde hemen değişiklik yapamayabilirsiniz; 4 saat bekleyin ve yeni oluşturulan bir ilkeyi yeniden değiştirmeye çalışın.</span><span class="sxs-lookup"><span data-stu-id="eb3df-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="eb3df-113">Hala sorun yaşıyorsanız PowerShell'i deneyin.</span><span class="sxs-lookup"><span data-stu-id="eb3df-113">If you're still having problems, try PowerShell.</span></span>  