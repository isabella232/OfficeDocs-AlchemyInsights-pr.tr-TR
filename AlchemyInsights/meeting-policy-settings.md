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
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704626"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Microsoft Teams'de toplantı ilkelerini yönetme

**Not: İlke değişikliklerinin kullanıcılar için etkili bir şekilde 24 saat kadar sürebilir.** Yeni oluşturulan ilkelerde hemen değişiklik yapmayabileceksiniz; 4 saat bekleyin ve yeni oluşturulan ilkeyi yeniden değiştirmeyi deneyin.

Toplantı ilkeleri, kuruluşta kullanıcılar tarafından zamanlanan toplantılarda toplantı katılımcılarına kullanılabilen özellikleri kontrol etmek için kullanılır. Toplantı ilkelerinin bazı özellikleri henüz Teams yönetim merkezinde uygulanmamış olabilir (bunlar, belgelerde "çok yakında" olarak etiketlenmiş olabilir). Bu durumda veya Microsoft Teams yönetim merkezinde "İlkeyi şu anda güncelleştireemedik ancak daha sonra yeniden deneyin" gibi bir hata alıyorsanız, Teams toplantı ilkeleri oluşturmak veya değiştirmek için PowerShell'i kullanmanızı öneririz. 

Toplantı ilkeleri hakkında daha fazla bilgi için aşağıdaki kaynaklara bakın:

- İlke oluşturma, değişiklik yapma ve kullanıcıları ilkeye atama hakkında bilgi edinmek için [Bkz. Teams'de toplantı ilkelerini yönetme.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- PowerShell cmdlet'lerini kullanarak ilke değişiklikleri yapmak için [Teams PowerShell'e Genel Bakış'a bakın.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Teams toplantı ilkeleri için [Skype Kurumsal PowerShell modülünü](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) kullanmalıdır. 
    - Daha fazla [bilgi için *-CsTeamsMeetingPolicy cmdlet'lerinin](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) belgelerini gözden geçirebilirsiniz.

