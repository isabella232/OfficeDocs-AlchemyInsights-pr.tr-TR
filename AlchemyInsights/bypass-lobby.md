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
ms.openlocfilehash: 6632bb0c09c7ce99f14cd55582025b37a846369d
ms.sourcegitcommit: ee719f011f766fc20d23e935e98d7e33c326183b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37654276"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Lobi ayarlarını ve katılım düzeyini kontrol edin

Çevirmeli, harici ve anonim kullanıcılar da dahil olmak üzere herkesin lobiyi atlamasına izin vermek istiyorsanız, bunu yapmak için PowerShell'i kullanabilirsiniz. Kuruluşunuz için genel toplantı ilkesini değiştirmenize bir örnek aşağıda verilmiştir:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Bu cmdlet şu anda Skype for Business PowerShell modülü kullanımını gerektirir. Bu cmdlet'i kullanmak için kurulum almak için [PowerShell üzerinden politikaları yönetme'ye](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)göz atın.

Daha sonra kullanıcılara uygulamanız gereken yeni bir ilke ayarlayabilirsiniz. Genel politikayı değiştirirseniz, kullanıcılar için otomatik olarak geçerli olur. Herhangi bir ilke değişikliği için, ilkelerin etkili olması için en az 4 saat ve 24 saat ekadar beklemeniz gerekir.

Bunun tam olarak nelere izin verdiğini anlamak için bu değişiklikleri yapmadan önce aşağıdaki belgeleri gözden geçirdiğinizden emin olun.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Lobi politikası denetimlerini karşılayan Ekipleri Anlama

- [İnsanların](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) doğrudan bir toplantıya katılıp katılmadıklarını veya kimlik doğrulaması yapılan bir kullanıcı tarafından kabul edilene kadar lobide bekleyip beklemediklerini kontrol eden bir düzenleyici başına ilke olduğunu otomatik olarak kabul edin.

- [Anonim kişilerin toplantı başlatmasına izin vermek,](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) B2B ve federe kullanıcılar da dahil olmak üzere anonim kişilerin, kuruluşun kimliği doğrulanmış bir kullanıcısı olmadan kullanıcının toplantısına katılıp katılamadığını kontrol eden bir düzenleyici başına ilkedir.

- [Arayarak gelen kullanıcıların lobiyi atlamasına izin verin](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(yakında)** telefonla arayan kişilerin toplantıya doğrudan katılıp katılmadığını veya otomatik olarak **kabul** edilen kişileri otomatik olarak kabul etmelerine bakılmaksızın lobide bekleyip beklemediğini kontrol eden bir düzenleyici başına politikadır.

- [Organizatörlerin lobi ayarlarını geçersiz kılmasına izin vermek](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(yakında)** toplantı düzenleyicisinin, bir yöneticinin **otomatik olarak kişileri kabul** ettiği lobi ayarlarını geçersiz kılıp geçersiz kılamayacağını kontrol eden ve **arayarak bağlanmaya izin veren bir ilkedir kullanıcılar** yeni bir toplantı zamanladıklarında lobiyi atlarlar.

**Not:** Microsoft Teams toplantı ilkelerine tam bir genel bakış için [Ekipler'deki toplantı ilkelerini yönet'i](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) okuyun.
