---
title: Toplantı ilkesi ayarları
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794354"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Microsoft ekiplerde toplantı ilkelerini yönetme

**Not: ilke değişikliklerinin kullanıcılar için geçerli olması 24 saate kadar sürebilir.** Yeni oluşturulan ilkelerde hemen değişiklik yapamayabilirsiniz; 4 saat bekleyin ve yeni oluşturulan bir ilkeyi yeniden değiştirmeyi deneyin.

Toplantı ilkeleri, kuruluşunuzdaki kullanıcılar tarafından zamanlanmış toplantılar için toplantı katılımcılarının kullanabildiği özellikleri denetlemek için kullanılır. Toplantı ilkelerinin bazı özellikleri ekiplerin Yönetim merkezinde henüz uygulanmayabilir (Bunlar, belgede "çok yakında" etiketlenir). Bu durumda ya da "ilkeyi Şu anda güncelleştiremiyoruz, ancak daha sonra tekrar denemeniz" gibi bir hata alıyorsanız, ekip toplantısı ilkelerini oluşturmak veya değiştirmek için PowerShell kullanmanızı öneririz. 

Toplantı ilkeleri hakkında daha fazla bilgi için aşağıdaki kaynaklara bakın:

- İlke oluşturma, değişiklik yapma ve ilkeye Kullanıcı atama hakkında bilgi edinmek için [ekiplerde toplantı Ilkelerini yönetme](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)bölümüne bakın.

- PowerShell cmdlet 'lerini kullanarak ilke değişiklikleri yapmak için, [bkz.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Ekip toplantısı için Skype Kurumsal [PowerShell modülünü](https://www.microsoft.com/download/details.aspx?id=39366) kullanmanız gerekir. 
    - Daha fazla bilgi için [*-csteamsmeeting ingpolicy cmdlet belgelerini](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) gözden geçirin.

