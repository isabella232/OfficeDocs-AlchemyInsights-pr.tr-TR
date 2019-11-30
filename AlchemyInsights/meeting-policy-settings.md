---
title: İlke ayarlarını karşılama
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627594"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Microsoft Teams'de toplantı ilkelerini yönetme

Toplantı ilkeleri, kuruluşunuzdaki kullanıcılar tarafından zamanlanan toplantılar için toplantı katılımcıları için kullanılabilen özellikleri denetlemek için kullanılır. Toplantı ilkelerinin bazı özellikleri henüz Takımlar yönetici merkezinde uygulanmayabilir (bunlar belgelerde "yakında" olarak etiketlenir). Bu durumda veya Microsoft Teams yönetici merkezinde "İlkeyi şu anda güncelleştiremeyiz, ancak daha sonra tekrar deneyin" gibi bir hata alıyorsanız, Ekipler toplantı ilkeleri oluşturmak veya değiştirmek için PowerShell'i kullanmanızı öneririz. 

Toplantı ilkeleri hakkında daha fazla bilgi için aşağıdaki kaynaklara bakın:

- İlkeler oluşturma, değişiklik yapma ve kullanıcıları ilkeye atama hakkında bilgi edinmek için [Bkz. Ekipler'deki toplantı ilkelerini yönet.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- PowerShell cmdlets kullanarak politika değişiklikleri yapmak için [Bkz. Teams PowerShell Genel Bakış.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Ekipler toplantı ilkeleri için [Skype for Business PowerShell modüllerini](https://www.microsoft.com/download/details.aspx?id=39366) kullanmanız gerekir. 
    - Daha fazla bilgi için [*-CsTeamsMeetingPolicy cmdlets belgelerini](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) inceleyin.

**Not:** İlke değişikliklerinin kullanıcılar için geçerli olması 24 saat kadar sürebilir. Yeni oluşturulan ilkelerde hemen değişiklik yapamayabilirsiniz; 4 saat bekleyin ve yeni oluşturulan bir ilkeyi yeniden değiştirmeye çalışın. Hala sorun yaşıyorsanız PowerShell'i deneyin.  