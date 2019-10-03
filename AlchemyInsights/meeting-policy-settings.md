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
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376880"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Microsoft Teams'de toplantı ilkelerini yönetme

Toplantı ilkeleri, kuruluşunuzdaki kullanıcılar tarafından zamanlanan toplantılar için toplantı katılımcıları için kullanılabilen özellikleri denetlemek için kullanılır. Toplantı ilkelerinin bazı özellikleri henüz Takımlar yönetici merkezinde uygulanmayabilir (bunlar belgelerde "yakında" olarak etiketlenir). Bu durumda veya Microsoft Teams yönetici merkezinde "İlkeyi şu anda güncelleştiremeyiz, ancak daha sonra tekrar deneyin" gibi bir hata alıyorsanız, Ekipler toplantı ilkeleri oluşturmak veya değiştirmek için PowerShell'i kullanmanızı öneririz. 

Toplantı ilkeleri hakkında daha fazla bilgi için aşağıdaki kaynaklara bakın:

- İlkeler oluşturma, değişiklik yapma ve kullanıcıları ilkeye atama hakkında bilgi edinmek için [Bkz. Ekipler'deki toplantı ilkelerini yönet.](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)

- PowerShell cmdlets kullanarak politika değişiklikleri yapmak için [Bkz. Teams PowerShell Genel Bakış.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Ekipler toplantı ilkeleri için [Skype for Business PowerShell modüllerini](https://www.microsoft.com/download/details.aspx?id=39366) kullanmanız gerekir. 
    - Daha fazla bilgi için [*-CsTeamsMeetingPolicy cmdlets belgelerini](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) inceleyin.

**Not:** İlke değişikliklerinin kullanıcılar için geçerli olması 24 saat kadar sürebilir. Yeni oluşturulan ilkelerde hemen değişiklik yapamayabilirsiniz; 4 saat bekleyin ve yeni oluşturulan bir ilkeyi yeniden değiştirmeye çalışın. Hala sorun yaşıyorsanız PowerShell'i deneyin.  