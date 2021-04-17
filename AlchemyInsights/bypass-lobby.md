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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Teams'te lobi ayarlarını ve katılım düzeyini denetleme

Arayarak bağlanılan, dış ve anonim kullanıcılar dahil herkesin lobiyi atlayarak bu görevi gerçekleştirmesine izin vermek için PowerShell'i kullanın. İşte, genel toplantı ilkesi ayarlarının kurum için değiştirilmesi için bir örnek.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Bu cmdlet, şu anda Skype Kurumsal PowerShell modülünün kullanımını gerektirir. Bu cmdlet'i kullanmak üzere ayarlamak için, [PowerShell aracılığıyla ilkeleri yönetme'ye göz atabilirsiniz.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

bir ilkeyi ayar defa kullanıcılara uygulayabilirsiniz; veya Genel ilkesi değiştirildiyseniz, otomatik olarak kullanıcılara uygulanır. İlke değişikliğinin yürürlüğe girecekleri en az **4 saat ile 24** saat arasında beklemenız gerekir. 

Bunun tam olarak neleri izin yaptığını anlamak için bu değişiklikleri yapmadan önce aşağıdaki belgeleri gözden geçirmeyi deneyin.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Teams toplantı lobisi ilke denetimlerini anlama

Bu ayarlar, toplantıya kabul edilen toplantı katılımcılarını ve bir toplantıya katılım düzeyini kontrol sağlar. Henüz uygulanmamış toplantı ilkesi ayarlarını (Teams yönetim merkezinde "çok yakında" etiketli) güncelleştirmek için PowerShell'i kullanabilirsiniz. Tüm kullanıcıların lobiyi atlaymalarını sağlayan örnek PowerShell cmdlet'i için aşağıya bakın.

- [Kişilerin otomatik olarak kabul](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) etmek, kişilerin toplantıya doğrudan mı katılacağını yoksa kimliği doğrulanmış bir kullanıcı tarafından kabul edilene kadar lobide mi bekleyeceğini kontrol eden düzenleyici başına bir ilkedir.

- [Anonim](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) kişilerin toplantı başlatmasına izin verme, B2B ve federasyon kullanıcıları dahil olmak üzere anonim kişilerin, kuruluştan kimliği doğrulanmış bir kullanıcı yoklamadan kullanıcının toplantısına katılıp katılamayebileceğini kontrol eden düzenleyici başına bir ilkedir.

- [Arayarak bağlanılan](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) kullanıcıların lobiyi atlamalarına **izin** ver (çok yakında), Telefonla arayarak bağlanılan kişilerin toplantıya doğrudan mı katılacağını yoksa Otomatik olarak kişi kabul et ayarına bakılmaksızın lobide mi bekleyeceğini kontrol eden, düzenleyici başına bir **ilkedir.**

- [Düzenleyicilerin](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) lobi ayarlarını geçersiz k olmasına izin ver **(çok** yakında), yöneticinin Otomatik olarak kişi kabul  et ve  Arayarak bağlanılan kullanıcıların yeni bir toplantı zamanlaması sırasında lobiyi atlaması için izin ver ayarında ayarlayan lobi ayarlarını geçersiz kıp et etebileceğini kontrol eden, düzenleyici başına bir ilkedir.

**Not:** Microsoft [Teams toplantı ilkelerine tam bir](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) genel bakış için Teams'de toplantı ilkelerini yönetme makalesinde okuyabilirsiniz.
