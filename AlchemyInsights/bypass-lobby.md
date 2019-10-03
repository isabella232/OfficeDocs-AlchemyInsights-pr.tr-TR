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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376885"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="1b703-102">Lobi ayarlarını ve katılım düzeyini kontrol edin</span><span class="sxs-lookup"><span data-stu-id="1b703-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="1b703-103">Bu ayarlar, toplantı katılımcılarının toplantıya kabul edilmeden önce lobide hangi toplantıyı beklediklerini ve toplantıya katılmalarına izin verilen katılım düzeyini kontrol altına almaktadır.</span><span class="sxs-lookup"><span data-stu-id="1b703-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="1b703-104">Powershell'i, Takımlar yönetici merkezinde henüz uygulanmamış ("yakında" olarak etiketlenmiş) toplantı ilkesi ayarlarını güncelleştirmek için kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1b703-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="1b703-105">Tüm kullanıcıların lobiyi atlamasına izin veren bir örnek PowerShell cmdlet için aşağıya bakın.</span><span class="sxs-lookup"><span data-stu-id="1b703-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="1b703-106">[İnsanların](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) doğrudan bir toplantıya katılıp katılmadıklarını veya kimlik doğrulaması yapılan bir kullanıcı tarafından kabul edilene kadar lobide bekleyip beklemediklerini kontrol eden bir düzenleyici başına ilke olduğunu otomatik olarak kabul edin.</span><span class="sxs-lookup"><span data-stu-id="1b703-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="1b703-107">[Anonim kişilerin toplantı başlatmasına izin vermek,](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) B2B ve federe kullanıcılar da dahil olmak üzere anonim kişilerin, kuruluşun kimliği doğrulanmış bir kullanıcısı olmadan kullanıcının toplantısına katılıp katılamadığını kontrol eden bir düzenleyici başına ilkedir.</span><span class="sxs-lookup"><span data-stu-id="1b703-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="1b703-108">[Arayarak gelen kullanıcıların lobiyi atlamasına izin verin](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(yakında)** telefonla arayan kişilerin toplantıya doğrudan katılıp katılmadığını veya otomatik olarak **kabul** edilen kişileri otomatik olarak kabul etmelerine bakılmaksızın lobide bekleyip beklemediğini kontrol eden bir düzenleyici başına politikadır.</span><span class="sxs-lookup"><span data-stu-id="1b703-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="1b703-109">[Organizatörlerin lobi ayarlarını geçersiz kılmasına izin vermek](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(yakında)** toplantı düzenleyicisinin, bir yöneticinin **otomatik olarak kişileri kabul** ettiği lobi ayarlarını geçersiz kılıp geçersiz kılamayacağını kontrol eden ve **arayarak bağlanmaya izin veren bir ilkedir kullanıcılar** yeni bir toplantı zamanladıklarında lobiyi atlarlar.</span><span class="sxs-lookup"><span data-stu-id="1b703-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="1b703-110">**Not:** Microsoft Teams toplantı ilkelerine tam bir genel bakış için [Ekipler'deki toplantı ilkelerini yönet'i](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) okuyun.</span><span class="sxs-lookup"><span data-stu-id="1b703-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="1b703-111">**PowerShell örneği**</span><span class="sxs-lookup"><span data-stu-id="1b703-111">**PowerShell example**</span></span>

<span data-ttu-id="1b703-112">Harici veya anonim kullanıcılar da dahil olmak üzere herkesin lobiyi atlamasına izin vermek isterseniz, bu görevi gerçekleştirmek için PowerShell'i de kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1b703-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="1b703-113">Aşağıda, kuruluşunuz için genel toplantı ilkesini değiştirmenin bir örneği verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="1b703-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="1b703-114">(Bu değişikliklerin tam olarak nelere izin verdiğini anlamak için bu değişiklikleri yapmadan önce yukarıdaki belgeleri gözden geçirin.)</span><span class="sxs-lookup"><span data-stu-id="1b703-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="1b703-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Herkes" -AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="1b703-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="1b703-116">Daha fazla bilgi için [Set-CsTeamsMeetingPolicy'ye](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps)bakın.</span><span class="sxs-lookup"><span data-stu-id="1b703-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
