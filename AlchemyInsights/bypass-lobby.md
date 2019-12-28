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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Kontrol lobisi ayarları ve Takımlara katılım düzeyi

Çevirmeli, harici ve anonim kullanıcılar da dahil olmak üzere herkesin **lobiyi atlamasına**izin vermek istiyorsanız, bu görevi gerçekleştirmek için PowerShell'i kullanın. Aşağıda, kuruluşunuz için genel toplantı ilkesini değiştirmenin bir örneği verilmiştir.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Bu cmdlet şu anda Skype for Business PowerShell modülü kullanımını gerektirir. Bu cmdlet'i kullanmak için kurulum yapmak için [PowerShell üzerinden yönetme politikalarına](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)göz atın.

Bir ilke ayarladıktan sonra, bu politikayı kullanıcılara uygulamanız gerekir; veya Genel politikayı değiştirdiyseniz, bu politika kullanıcılar için otomatik olarak geçerli olacaktır. Herhangi bir ilke değişikliği için, ilkelerin etkili olması için en az **4 saat ila 24 saat** beklemeniz gerekir. 

Bunun tam olarak nelere izin verdiğini anlamak için bu değişiklikleri yapmadan önce aşağıdaki belgeleri gözden geçirdiğinizden emin olun.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Lobi politikası denetimlerini karşılayan Ekipleri Anlama

Bu ayarlar, toplantı katılımcılarının toplantıya kabul edilmeden önce lobide hangi toplantıyı beklediklerini ve toplantıya katılmalarına izin verilen katılım düzeyini kontrol altına almaktadır. PowerShell'i, Takımlar yönetici merkezinde henüz uygulanmamış ("yakında" olarak etiketlenmiş) toplantı ilkesi ayarlarını güncelleştirmek için kullanabilirsiniz. Tüm kullanıcıların lobiyi atlamasına izin veren bir örnek PowerShell cmdlet için aşağıya bakın.

- [İnsanların](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) doğrudan bir toplantıya katılıp katılmadıklarını veya kimlik doğrulaması yapılan bir kullanıcı tarafından kabul edilene kadar lobide bekleyip beklemediklerini kontrol eden bir düzenleyici başına ilke olduğunu otomatik olarak kabul edin.

- [Anonim kişilerin toplantı başlatmasına izin vermek,](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) B2B ve federe kullanıcılar da dahil olmak üzere anonim kişilerin, kuruluşun kimliği doğrulanmış bir kullanıcısı olmadan kullanıcının toplantısına katılıp katılamadığını kontrol eden bir düzenleyici başına ilkedir.

- [Arayarak gelen kullanıcıların lobiyi atlamasına izin verin](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(yakında)** telefonla arayan kişilerin toplantıya doğrudan katılıp katılmadığını veya otomatik olarak **kabul** edilen kişileri otomatik olarak kabul etmelerine bakılmaksızın lobide bekleyip beklemediğini kontrol eden bir düzenleyici başına politikadır.

- [Organizatörlerin lobi ayarlarını geçersiz kılmasına izin vermek](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(yakında)** toplantı düzenleyicisinin, bir yöneticinin **otomatik olarak ayarlanan kişileri kabul** ettiği lobi ayarlarını geçersiz kılıp geçersiz kılıp geçersiz kılamayacağını kontrol eden ve arayarak gelen kullanıcıların yeni bir toplantı planladıklarında **lobiyi atlamalarına izin** veren bir ilkedir.

**Not:** Microsoft Teams toplantı ilkelerine tam bir genel bakış için [Ekipler'deki toplantı ilkelerini yönet'i](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) okuyun.
