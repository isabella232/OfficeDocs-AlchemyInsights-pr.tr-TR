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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Ekipte ekip ayarlarını ve katılım düzeyini denetleme

Arayarak bağlanılan, dış ve anonim kullanıcılar dahil herkese izin **vermek istiyorsanız,** bu görevi gerçekleştirmek için PowerShell kullanın. Kuruluşunuzun genel toplantı ilkesini değiştirme örneği aşağıdadır.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Bu cmdlet 'in şimdilik Skype Kurumsal PowerShell modülünü kullanması gerekir. Bu cmdlet 'i kullanacak şekilde ayarlamak için, [PowerShell aracılığıyla Ilkelerin yönetimini](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)inceleyin.

Bir ilke ayarladıktan sonra kullanıcılara uygulamanız gerekir; veya genel ilkesini değiştirdiyseniz, otomatik olarak kullanıcılara uygulanır. Tüm ilke değişiklikleri için, ilkelerin geçerlilik kazanması en az **4 saat 24 saate kadar** beklemeniz gerekir. 

Bu değişikliklerin tam olarak nasıl izin verdiğini anlamak için aşağıdaki belgeleri gözden geçirmeyi unutmayın.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Ekip toplantısı toplantısı ilkesi denetimlerini anlama

Bu ayarlar, toplantıya kabul edilmeden önce hangi toplantı katılımcılarının lobide beklediklerini ve toplantıda izin verilen katılım düzeyini denetler. Ekip yönetim merkezinde henüz uygulanmamış ("çok yakında" etiketlenen) toplantı ilkesi ayarlarını güncelleştirmek için PowerShell 'i kullanabilirsiniz. Tüm kullanıcıların lobiyi atlamasına olanak tanıyan örnek bir PowerShell cmdlet 'ini görün.

- [Kişiler otomatik olarak](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , kişilerin bir toplantıya doğrudan katılıp katılmadığını ya da kimliği doğrulanmış bir kullanıcı tarafından kabul edilene kadar lobide beklemesini denetler.

- [Anonim kişilerin toplantıyı başlatmalarına Izin verme](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , B2B ve Federasyon kullanıcıları dahil olmak üzere anonim kişilerin Kullanıcı toplantısına, toplantıya katılımcı bir kullanıcı olmaksızın katılabilirler.

- [Arayarak bağlanılan kullanıcıların lobiyi atlamasına izin ver](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (çok**yakında**) telefon ile arayarak bağlanan kişilerin toplantıya doğrudan katılmasını veya **otomatik olarak lobideki kişi** ayarını dikkate almaksızın lobide beklemesini denetleyen düzenleyici

- [Düzenleyicilerin lobma ayarlarını geçersiz kılmasına Izin ver](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (çok**yakında**), toplantıyı düzenleyenin, **kişiler için otomatik olarak** ayarlanan bir yöneticinin giriş ayarlarını geçersiz kılmasını ve arayarak bağlanılan kullanıcıların yeni bir toplantı zamanlarken **lobide atlamasına izin** verip vermediğini denetleyen bir düzenleyici politikadır.

**Not:** Microsoft ekipleri toplantı ilkelerine eksiksiz bir genel bakış için [ekipte toplantı Ilkelerini yönetin](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) bölümünü okuyun.
