---
title: Belirli Exchange Online dkIM'yi etkinleştirmek için PowerShell'i kullanma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070344"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Belirli Exchange Online dkIM'yi etkinleştirmek için PowerShell'i kullanma

Yönetim merkezinde DKIM DNS kayıtlarını oluştura değilseniz, Exchange Online PowerShell kullanmayı deneyin. 

Exchange Online PowerShell kullanarak DKIM DNS kaydı oluşturmak için aşağıdaki adımları gerçekleştirin:

1. Görev Windows PowerShell yönetici olarak açın ve açıklanan sırayla aşağıdaki komutları çalıştırın:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Exchange Online PowerShell'e bağlanırken sorun Exchange Online, [bkz. Bağlan PowerShell'Exchange Online.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Exchange Online PowerShell'e bağlandıktan sonra aşağıdaki komutu çalıştırın:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Yukarıdaki komut başarıyla çalıştırılana kadar, aşağıdaki komutu çalıştırarak Exchange Online PowerShell oturumunu sonlandırın:

    `Remove-PSSession $Session` 



