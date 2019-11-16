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
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768460"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="1df1a-102">Lobi ayarlarını ve katılım düzeyini kontrol edin</span><span class="sxs-lookup"><span data-stu-id="1df1a-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="1df1a-103">Arayarak, harici ve anonim kullanıcılar da dahil olmak üzere herkesin Microsoft Teams'teki lobiyi atlamasına izin vermek isterseniz, bunu yapmak için PowerShell'i kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1df1a-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby in Microsoft Teams, you can use PowerShell to do it.</span></span> <span data-ttu-id="1df1a-104">Kuruluşunuz için genel toplantı ilkesini değiştirmenize bir örnek aşağıda verilmiştir:</span><span class="sxs-lookup"><span data-stu-id="1df1a-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="1df1a-105">Bu cmdlet şu anda Skype for Business PowerShell modülü kullanımını gerektirir.</span><span class="sxs-lookup"><span data-stu-id="1df1a-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="1df1a-106">Bu cmdlet'i kullanmak için kurulum almak için [PowerShell üzerinden politikaları yönetme'ye](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)göz atın.</span><span class="sxs-lookup"><span data-stu-id="1df1a-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="1df1a-107">Daha sonra kullanıcılara uygulamanız gereken yeni bir ilke ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1df1a-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="1df1a-108">Genel politikayı değiştirirseniz, kullanıcılar için otomatik olarak geçerli olur.</span><span class="sxs-lookup"><span data-stu-id="1df1a-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="1df1a-109">Herhangi bir ilke değişikliği için, ilkelerin etkili olması için en az 4 saat ve 24 saat ekadar beklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="1df1a-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="1df1a-110">Bunun tam olarak nelere izin verdiğini anlamak için bu değişiklikleri yapmadan önce aşağıdaki belgeleri gözden geçirdiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="1df1a-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="1df1a-111">Lobi politikası denetimlerini karşılayan Ekipleri Anlama</span><span class="sxs-lookup"><span data-stu-id="1df1a-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="1df1a-112">[İnsanların](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) doğrudan bir toplantıya katılıp katılmadıklarını veya kimlik doğrulaması yapılan bir kullanıcı tarafından kabul edilene kadar lobide bekleyip beklemediklerini kontrol eden bir düzenleyici başına ilke olduğunu otomatik olarak kabul edin.</span><span class="sxs-lookup"><span data-stu-id="1df1a-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="1df1a-113">[Anonim kişilerin toplantı başlatmasına izin vermek,](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) B2B ve federe kullanıcılar da dahil olmak üzere anonim kişilerin, kuruluşun kimliği doğrulanmış bir kullanıcısı olmadan kullanıcının toplantısına katılıp katılamadığını kontrol eden bir düzenleyici başına ilkedir.</span><span class="sxs-lookup"><span data-stu-id="1df1a-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="1df1a-114">[Arayarak gelen kullanıcıların lobiyi atlamasına izin verin](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(yakında)** telefonla arayan kişilerin toplantıya doğrudan katılıp katılmadığını veya otomatik olarak **kabul** edilen kişileri otomatik olarak kabul etmelerine bakılmaksızın lobide bekleyip beklemediğini kontrol eden bir düzenleyici başına politikadır.</span><span class="sxs-lookup"><span data-stu-id="1df1a-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="1df1a-115">[Organizatörlerin lobi ayarlarını geçersiz kılmasına izin vermek](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(yakında)** toplantı düzenleyicisinin, bir yöneticinin **otomatik olarak ayarlanan kişileri kabul** ettiği lobi ayarlarını geçersiz kılıp geçersiz kılıp geçersiz kılamayacağını kontrol eden ve arayarak gelen kullanıcıların yeni bir toplantı planladıklarında **lobiyi atlamalarına izin** veren bir ilkedir.</span><span class="sxs-lookup"><span data-stu-id="1df1a-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="1df1a-116">**Not:** Microsoft Teams toplantı ilkelerine tam bir genel bakış için [Ekipler'deki toplantı ilkelerini yönet'i](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) okuyun.</span><span class="sxs-lookup"><span data-stu-id="1df1a-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
