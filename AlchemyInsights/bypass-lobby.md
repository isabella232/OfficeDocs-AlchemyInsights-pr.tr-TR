---
title: Lobiyi atla
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684970"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="92612-102">Ekipte ekip ayarlarını ve katılım düzeyini denetleme</span><span class="sxs-lookup"><span data-stu-id="92612-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="92612-103">Arayarak bağlanılan, dış ve anonim kullanıcılar dahil herkese izin **vermek istiyorsanız,** bu görevi gerçekleştirmek için PowerShell kullanın.</span><span class="sxs-lookup"><span data-stu-id="92612-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="92612-104">Kuruluşunuzun genel toplantı ilkesini değiştirme örneği aşağıdadır.</span><span class="sxs-lookup"><span data-stu-id="92612-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="92612-105">Bu cmdlet 'in şimdilik Skype Kurumsal PowerShell modülünü kullanması gerekir.</span><span class="sxs-lookup"><span data-stu-id="92612-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="92612-106">Bu cmdlet 'i kullanacak şekilde ayarlamak için, [PowerShell aracılığıyla Ilkelerin yönetimini](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)inceleyin.</span><span class="sxs-lookup"><span data-stu-id="92612-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="92612-107">Bir ilke ayarladıktan sonra kullanıcılara uygulamanız gerekir; veya genel ilkesini değiştirdiyseniz, otomatik olarak kullanıcılara uygulanır.</span><span class="sxs-lookup"><span data-stu-id="92612-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="92612-108">Tüm ilke değişiklikleri için, ilkelerin geçerlilik kazanması en az **4 saat 24 saate kadar** beklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="92612-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="92612-109">Bu değişikliklerin tam olarak nasıl izin verdiğini anlamak için aşağıdaki belgeleri gözden geçirmeyi unutmayın.</span><span class="sxs-lookup"><span data-stu-id="92612-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="92612-110">Ekip toplantısı toplantısı ilkesi denetimlerini anlama</span><span class="sxs-lookup"><span data-stu-id="92612-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="92612-111">Bu ayarlar, toplantıya kabul edilmeden önce hangi toplantı katılımcılarının lobide beklediklerini ve toplantıda izin verilen katılım düzeyini denetler.</span><span class="sxs-lookup"><span data-stu-id="92612-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="92612-112">Ekip yönetim merkezinde henüz uygulanmamış ("çok yakında" etiketlenen) toplantı ilkesi ayarlarını güncelleştirmek için PowerShell 'i kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="92612-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="92612-113">Tüm kullanıcıların lobiyi atlamasına olanak tanıyan örnek bir PowerShell cmdlet 'ini görün.</span><span class="sxs-lookup"><span data-stu-id="92612-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="92612-114">[Kişiler otomatik olarak](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , kişilerin bir toplantıya doğrudan katılıp katılmadığını ya da kimliği doğrulanmış bir kullanıcı tarafından kabul edilene kadar lobide beklemesini denetler.</span><span class="sxs-lookup"><span data-stu-id="92612-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="92612-115">[Anonim kişilerin toplantıyı başlatmalarına Izin verme](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , B2B ve Federasyon kullanıcıları dahil olmak üzere anonim kişilerin Kullanıcı toplantısına, toplantıya katılımcı bir kullanıcı olmaksızın katılabilirler.</span><span class="sxs-lookup"><span data-stu-id="92612-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="92612-116">[Arayarak bağlanılan kullanıcıların lobiyi atlamasına izin ver](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (çok**yakında**) telefon ile arayarak bağlanan kişilerin toplantıya doğrudan katılmasını veya **otomatik olarak lobideki kişi** ayarını dikkate almaksızın lobide beklemesini denetleyen düzenleyici</span><span class="sxs-lookup"><span data-stu-id="92612-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="92612-117">[Düzenleyicilerin lobma ayarlarını geçersiz kılmasına Izin ver](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (çok**yakında**), toplantıyı düzenleyenin, **kişiler için otomatik olarak** ayarlanan bir yöneticinin giriş ayarlarını geçersiz kılmasını ve arayarak bağlanılan kullanıcıların yeni bir toplantı zamanlarken **lobide atlamasına izin** verip vermediğini denetleyen bir düzenleyici politikadır.</span><span class="sxs-lookup"><span data-stu-id="92612-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="92612-118">**Not:** Microsoft ekipleri toplantı ilkelerine eksiksiz bir genel bakış için [ekipte toplantı Ilkelerini yönetin](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) bölümünü okuyun.</span><span class="sxs-lookup"><span data-stu-id="92612-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
