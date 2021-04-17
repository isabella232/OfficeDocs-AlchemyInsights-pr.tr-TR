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
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825463"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Microsoft Teams'de toplantı ilkelerini yönetme

**Not: İlke değişikliklerinin kullanıcılarda etkiliksi 24 saate kadar sürebilir.** Yeni oluşturulan ilkelerde hemen değişiklik yapmayabileceksiniz; 4 saat bekleyin ve yeni oluşturulan ilkeyi yeniden değiştirmeyi deneyin.

Toplantı ilkeleri, kuruluşta kullanıcılar tarafından zamanlanan toplantılarda toplantı katılımcılarına kullanılabilen özellikleri denetlemede kullanılır. Toplantı ilkelerinin bazı özellikleri henüz Teams yönetim merkezinde uygulanmamış olabilir (bunlar, belgelerde "çok yakında" olarak etiketlenmiş olabilir). Bu durumda ya da Microsoft Teams yönetim merkezinde "İlkeyi şu anda güncelleştire miyiz" gibi bir hata alıyorsanız Teams toplantı ilkelerini oluşturmak veya değiştirmek için PowerShell'i kullanmanızı öneririz. 

Toplantı ilkeleri hakkında daha fazla bilgi için aşağıdaki kaynaklara bakın:

- İlke oluşturma, değişiklik yapma ve kullanıcıları ilkeye atama hakkında bilgi edinmek için bkz. [Teams'te toplantı ilkelerini yönetme.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- PowerShell cmdlet'lerini kullanarak ilke değişiklikleri yapmak için bkz. [Teams PowerShell'e Genel Bakış.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Teams toplantı ilkeleri için [Skype Kurumsal PowerShell modülünü](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) kullanmelisiniz. 
    - Daha fazla [bilgi için *-CsTeamsMeetingPolicy cmdlet'leri belgelerini](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) gözden geçirme.

