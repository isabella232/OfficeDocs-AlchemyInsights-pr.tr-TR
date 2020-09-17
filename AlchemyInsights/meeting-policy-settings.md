---
title: Toplantı ilkesi ayarları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794354"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="d1edf-102">Microsoft ekiplerde toplantı ilkelerini yönetme</span><span class="sxs-lookup"><span data-stu-id="d1edf-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="d1edf-103">**Not: ilke değişikliklerinin kullanıcılar için geçerli olması 24 saate kadar sürebilir.**</span><span class="sxs-lookup"><span data-stu-id="d1edf-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="d1edf-104">Yeni oluşturulan ilkelerde hemen değişiklik yapamayabilirsiniz; 4 saat bekleyin ve yeni oluşturulan bir ilkeyi yeniden değiştirmeyi deneyin.</span><span class="sxs-lookup"><span data-stu-id="d1edf-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="d1edf-105">Toplantı ilkeleri, kuruluşunuzdaki kullanıcılar tarafından zamanlanmış toplantılar için toplantı katılımcılarının kullanabildiği özellikleri denetlemek için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="d1edf-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="d1edf-106">Toplantı ilkelerinin bazı özellikleri ekiplerin Yönetim merkezinde henüz uygulanmayabilir (Bunlar, belgede "çok yakında" etiketlenir).</span><span class="sxs-lookup"><span data-stu-id="d1edf-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="d1edf-107">Bu durumda ya da "ilkeyi Şu anda güncelleştiremiyoruz, ancak daha sonra tekrar denemeniz" gibi bir hata alıyorsanız, ekip toplantısı ilkelerini oluşturmak veya değiştirmek için PowerShell kullanmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="d1edf-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="d1edf-108">Toplantı ilkeleri hakkında daha fazla bilgi için aşağıdaki kaynaklara bakın:</span><span class="sxs-lookup"><span data-stu-id="d1edf-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="d1edf-109">İlke oluşturma, değişiklik yapma ve ilkeye Kullanıcı atama hakkında bilgi edinmek için [ekiplerde toplantı Ilkelerini yönetme](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="d1edf-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="d1edf-110">PowerShell cmdlet 'lerini kullanarak ilke değişiklikleri yapmak için, [bkz.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="d1edf-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="d1edf-111">Ekip toplantısı için Skype Kurumsal [PowerShell modülünü](https://www.microsoft.com/download/details.aspx?id=39366) kullanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="d1edf-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="d1edf-112">Daha fazla bilgi için [\*-csteamsmeeting ingpolicy cmdlet belgelerini](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="d1edf-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

