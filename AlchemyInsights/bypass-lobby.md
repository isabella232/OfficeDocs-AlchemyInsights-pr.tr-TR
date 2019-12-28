---
title: Baypas lobisi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889102"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="80bb8-102">Kontrol lobisi ayarları ve Takımlara katılım düzeyi</span><span class="sxs-lookup"><span data-stu-id="80bb8-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="80bb8-103">Çevirmeli, harici ve anonim kullanıcılar da dahil olmak üzere herkesin **lobiyi atlamasına**izin vermek istiyorsanız, bu görevi gerçekleştirmek için PowerShell'i kullanın.</span><span class="sxs-lookup"><span data-stu-id="80bb8-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="80bb8-104">Aşağıda, kuruluşunuz için genel toplantı ilkesini değiştirmenin bir örneği verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="80bb8-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="80bb8-105">Bu cmdlet şu anda Skype for Business PowerShell modülü kullanımını gerektirir.</span><span class="sxs-lookup"><span data-stu-id="80bb8-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="80bb8-106">Bu cmdlet'i kullanmak için kurulum yapmak için [PowerShell üzerinden yönetme politikalarına](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)göz atın.</span><span class="sxs-lookup"><span data-stu-id="80bb8-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="80bb8-107">Bir ilke ayarladıktan sonra, bu politikayı kullanıcılara uygulamanız gerekir; veya Genel politikayı değiştirdiyseniz, bu politika kullanıcılar için otomatik olarak geçerli olacaktır.</span><span class="sxs-lookup"><span data-stu-id="80bb8-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="80bb8-108">Herhangi bir ilke değişikliği için, ilkelerin etkili olması için en az **4 saat ila 24 saat** beklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="80bb8-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="80bb8-109">Bunun tam olarak nelere izin verdiğini anlamak için bu değişiklikleri yapmadan önce aşağıdaki belgeleri gözden geçirdiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="80bb8-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="80bb8-110">Lobi politikası denetimlerini karşılayan Ekipleri Anlama</span><span class="sxs-lookup"><span data-stu-id="80bb8-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="80bb8-111">Bu ayarlar, toplantı katılımcılarının toplantıya kabul edilmeden önce lobide hangi toplantıyı beklediklerini ve toplantıya katılmalarına izin verilen katılım düzeyini kontrol altına almaktadır.</span><span class="sxs-lookup"><span data-stu-id="80bb8-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="80bb8-112">PowerShell'i, Takımlar yönetici merkezinde henüz uygulanmamış ("yakında" olarak etiketlenmiş) toplantı ilkesi ayarlarını güncelleştirmek için kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="80bb8-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="80bb8-113">Tüm kullanıcıların lobiyi atlamasına izin veren bir örnek PowerShell cmdlet için aşağıya bakın.</span><span class="sxs-lookup"><span data-stu-id="80bb8-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="80bb8-114">[İnsanların](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) doğrudan bir toplantıya katılıp katılmadıklarını veya kimlik doğrulaması yapılan bir kullanıcı tarafından kabul edilene kadar lobide bekleyip beklemediklerini kontrol eden bir düzenleyici başına ilke olduğunu otomatik olarak kabul edin.</span><span class="sxs-lookup"><span data-stu-id="80bb8-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="80bb8-115">[Anonim kişilerin toplantı başlatmasına izin vermek,](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) B2B ve federe kullanıcılar da dahil olmak üzere anonim kişilerin, kuruluşun kimliği doğrulanmış bir kullanıcısı olmadan kullanıcının toplantısına katılıp katılamadığını kontrol eden bir düzenleyici başına ilkedir.</span><span class="sxs-lookup"><span data-stu-id="80bb8-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="80bb8-116">[Arayarak gelen kullanıcıların lobiyi atlamasına izin verin](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(yakında)** telefonla arayan kişilerin toplantıya doğrudan katılıp katılmadığını veya otomatik olarak **kabul** edilen kişileri otomatik olarak kabul etmelerine bakılmaksızın lobide bekleyip beklemediğini kontrol eden bir düzenleyici başına politikadır.</span><span class="sxs-lookup"><span data-stu-id="80bb8-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="80bb8-117">[Organizatörlerin lobi ayarlarını geçersiz kılmasına izin vermek](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(yakında)** toplantı düzenleyicisinin, bir yöneticinin **otomatik olarak ayarlanan kişileri kabul** ettiği lobi ayarlarını geçersiz kılıp geçersiz kılıp geçersiz kılamayacağını kontrol eden ve arayarak gelen kullanıcıların yeni bir toplantı planladıklarında **lobiyi atlamalarına izin** veren bir ilkedir.</span><span class="sxs-lookup"><span data-stu-id="80bb8-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="80bb8-118">**Not:** Microsoft Teams toplantı ilkelerine tam bir genel bakış için [Ekipler'deki toplantı ilkelerini yönet'i](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) okuyun.</span><span class="sxs-lookup"><span data-stu-id="80bb8-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
