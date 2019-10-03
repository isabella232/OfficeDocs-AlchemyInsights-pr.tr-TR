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
# <a name="control-lobby-settings-and-level-of-participation"></a>Lobi ayarlarını ve katılım düzeyini kontrol edin

Bu ayarlar, toplantı katılımcılarının toplantıya kabul edilmeden önce lobide hangi toplantıyı beklediklerini ve toplantıya katılmalarına izin verilen katılım düzeyini kontrol altına almaktadır. Powershell'i, Takımlar yönetici merkezinde henüz uygulanmamış ("yakında" olarak etiketlenmiş) toplantı ilkesi ayarlarını güncelleştirmek için kullanabilirsiniz.  Tüm kullanıcıların lobiyi atlamasına izin veren bir örnek PowerShell cmdlet için aşağıya bakın.  

- [İnsanların](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) doğrudan bir toplantıya katılıp katılmadıklarını veya kimlik doğrulaması yapılan bir kullanıcı tarafından kabul edilene kadar lobide bekleyip beklemediklerini kontrol eden bir düzenleyici başına ilke olduğunu otomatik olarak kabul edin.

- [Anonim kişilerin toplantı başlatmasına izin vermek,](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) B2B ve federe kullanıcılar da dahil olmak üzere anonim kişilerin, kuruluşun kimliği doğrulanmış bir kullanıcısı olmadan kullanıcının toplantısına katılıp katılamadığını kontrol eden bir düzenleyici başına ilkedir.

- [Arayarak gelen kullanıcıların lobiyi atlamasına izin verin](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(yakında)** telefonla arayan kişilerin toplantıya doğrudan katılıp katılmadığını veya otomatik olarak **kabul** edilen kişileri otomatik olarak kabul etmelerine bakılmaksızın lobide bekleyip beklemediğini kontrol eden bir düzenleyici başına politikadır.

- [Organizatörlerin lobi ayarlarını geçersiz kılmasına izin vermek](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(yakında)** toplantı düzenleyicisinin, bir yöneticinin **otomatik olarak kişileri kabul** ettiği lobi ayarlarını geçersiz kılıp geçersiz kılamayacağını kontrol eden ve **arayarak bağlanmaya izin veren bir ilkedir kullanıcılar** yeni bir toplantı zamanladıklarında lobiyi atlarlar.

**Not:** Microsoft Teams toplantı ilkelerine tam bir genel bakış için [Ekipler'deki toplantı ilkelerini yönet'i](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) okuyun. 


**PowerShell örneği**

Harici veya anonim kullanıcılar da dahil olmak üzere herkesin lobiyi atlamasına izin vermek isterseniz, bu görevi gerçekleştirmek için PowerShell'i de kullanabilirsiniz.  Aşağıda, kuruluşunuz için genel toplantı ilkesini değiştirmenin bir örneği verilmiştir.   

(Bu değişikliklerin tam olarak nelere izin verdiğini anlamak için bu değişiklikleri yapmadan önce yukarıdaki belgeleri gözden geçirin.)

Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Herkes" -AllowPSTNUsersToBypassLobby $True

Daha fazla bilgi için [Set-CsTeamsMeetingPolicy'ye](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps)bakın.
