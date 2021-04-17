---
title: Lobiyi atlama
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820054"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="5e7b9-102">Teams'te lobi ayarlarını ve katılım düzeyini denetleme</span><span class="sxs-lookup"><span data-stu-id="5e7b9-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="5e7b9-103">Arayarak bağlanılan, dış ve anonim kullanıcılar dahil herkesin lobiyi atlayarak bu görevi gerçekleştirmesine izin vermek için PowerShell'i kullanın.</span><span class="sxs-lookup"><span data-stu-id="5e7b9-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="5e7b9-104">İşte, genel toplantı ilkesi ayarlarının kurum için değiştirilmesi için bir örnek.</span><span class="sxs-lookup"><span data-stu-id="5e7b9-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="5e7b9-105">Bu cmdlet, şu anda Skype Kurumsal PowerShell modülünün kullanımını gerektirir.</span><span class="sxs-lookup"><span data-stu-id="5e7b9-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="5e7b9-106">Bu cmdlet'i kullanmak üzere ayarlamak için, [PowerShell aracılığıyla ilkeleri yönetme'ye göz atabilirsiniz.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="5e7b9-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="5e7b9-107">bir ilkeyi ayar defa kullanıcılara uygulayabilirsiniz; veya Genel ilkesi değiştirildiyseniz, otomatik olarak kullanıcılara uygulanır.</span><span class="sxs-lookup"><span data-stu-id="5e7b9-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="5e7b9-108">İlke değişikliğinin yürürlüğe girecekleri en az **4 saat ile 24** saat arasında beklemenız gerekir.</span><span class="sxs-lookup"><span data-stu-id="5e7b9-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="5e7b9-109">Bunun tam olarak neleri izin yaptığını anlamak için bu değişiklikleri yapmadan önce aşağıdaki belgeleri gözden geçirmeyi deneyin.</span><span class="sxs-lookup"><span data-stu-id="5e7b9-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="5e7b9-110">Teams toplantı lobisi ilke denetimlerini anlama</span><span class="sxs-lookup"><span data-stu-id="5e7b9-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="5e7b9-111">Bu ayarlar, toplantıya kabul edilen toplantı katılımcılarını ve bir toplantıya katılım düzeyini kontrol sağlar.</span><span class="sxs-lookup"><span data-stu-id="5e7b9-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="5e7b9-112">Henüz uygulanmamış toplantı ilkesi ayarlarını (Teams yönetim merkezinde "çok yakında" etiketli) güncelleştirmek için PowerShell'i kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5e7b9-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="5e7b9-113">Tüm kullanıcıların lobiyi atlaymalarını sağlayan örnek PowerShell cmdlet'i için aşağıya bakın.</span><span class="sxs-lookup"><span data-stu-id="5e7b9-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="5e7b9-114">[Kişilerin otomatik olarak kabul](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) etmek, kişilerin toplantıya doğrudan mı katılacağını yoksa kimliği doğrulanmış bir kullanıcı tarafından kabul edilene kadar lobide mi bekleyeceğini kontrol eden düzenleyici başına bir ilkedir.</span><span class="sxs-lookup"><span data-stu-id="5e7b9-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="5e7b9-115">[Anonim](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) kişilerin toplantı başlatmasına izin verme, B2B ve federasyon kullanıcıları dahil olmak üzere anonim kişilerin, kuruluştan kimliği doğrulanmış bir kullanıcı yoklamadan kullanıcının toplantısına katılıp katılamayebileceğini kontrol eden düzenleyici başına bir ilkedir.</span><span class="sxs-lookup"><span data-stu-id="5e7b9-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="5e7b9-116">[Arayarak bağlanılan](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) kullanıcıların lobiyi atlamalarına **izin** ver (çok yakında), Telefonla arayarak bağlanılan kişilerin toplantıya doğrudan mı katılacağını yoksa Otomatik olarak kişi kabul et ayarına bakılmaksızın lobide mi bekleyeceğini kontrol eden, düzenleyici başına bir **ilkedir.**</span><span class="sxs-lookup"><span data-stu-id="5e7b9-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="5e7b9-117">[Düzenleyicilerin](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) lobi ayarlarını geçersiz k olmasına izin ver **(çok** yakında), yöneticinin Otomatik olarak kişi kabul  et ve  Arayarak bağlanılan kullanıcıların yeni bir toplantı zamanlaması sırasında lobiyi atlaması için izin ver ayarında ayarlayan lobi ayarlarını geçersiz kıp et etebileceğini kontrol eden, düzenleyici başına bir ilkedir.</span><span class="sxs-lookup"><span data-stu-id="5e7b9-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="5e7b9-118">**Not:** Microsoft [Teams toplantı ilkelerine tam bir](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) genel bakış için Teams'de toplantı ilkelerini yönetme makalesinde okuyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5e7b9-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
