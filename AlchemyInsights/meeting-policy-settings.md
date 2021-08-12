---
title: Toplantı ilkesi ayarları
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
- "9000734"
- "2657"
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925185"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Toplantıda toplantı ilkelerini Microsoft Teams

**Not: İlke değişikliklerinin kullanıcılarda etkiliksi 24 saate kadar sürebilir.** Yeni oluşturulan ilkelerde hemen değişiklik yapmayabileceksiniz; 4 saat bekleyin ve yeni oluşturulan ilkeyi yeniden değiştirmeyi deneyin.

Toplantı ilkeleri, kuruluşta kullanıcılar tarafından zamanlanan toplantılarda toplantı katılımcılarına kullanılabilen özellikleri denetlemede kullanılır. Toplantı ilkelerinin bazı özellikleri henüz yönetim merkezinde Teams (bunlar, belgelerde "çok yakında" olarak etiketlenmiş olabilir). Bu durumda veya Microsoft Teams yönetim merkezinde "İlkeyi şu anda güncelleştire miyiz" gibi bir hata alıyorsanız, toplantı ilkelerinizi oluşturmak veya değiştirmek için PowerShell Teams öneririz. 

Toplantı ilkeleri hakkında daha fazla bilgi için aşağıdaki kaynaklara bakın:

- İlke oluşturma, değişiklik yapma ve kullanıcıları ilkeye atama hakkında bilgi edinmek için bkz. [Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- PowerShell cmdlet'lerini kullanarak ilke değişiklikleri yapmak için bkz. [Teams PowerShell'e Genel Bakış](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Toplantı ilkelerini kullanmak [Skype Kurumsal PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) Teams gerekir. 
    - Daha fazla [bilgi için *-CsTeamsMeetingPolicy cmdlet'leri belgelerini](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) gözden geçirme.

