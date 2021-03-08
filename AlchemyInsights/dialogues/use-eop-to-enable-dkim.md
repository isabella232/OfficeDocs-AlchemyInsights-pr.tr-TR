---
title: Belirli bir etki alanı için DKIM'yi etkinleştirmek için Exchange Online PowerShell kullanma
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
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527220"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Belirli bir etki alanı için DKIM'yi etkinleştirmek için Exchange Online PowerShell kullanma

Yönetim merkezinde DKIM DNS kayıtlarını oluşturasanız, Exchange Online PowerShell kullanmayı deneyin. 

Exchange Online PowerShell kullanarak DKIM DNS kaydı oluşturmak için aşağıdaki adımları uygulayın:

1. Windows PowerShell'i yönetici olarak açın ve açıklanan sırayla aşağıdaki komutları çalıştırın:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Exchange Online PowerShell'e bağlanmada sorun varsa, [bkz. Exchange Online PowerShell'e Bağlanma.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Exchange Online PowerShell'e bağlandıktan sonra aşağıdaki komutu çalıştırın:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Yukarıdaki komut başarıyla yürütülürken, Exchange Online PowerShell oturumunu sonlandırmak için aşağıdaki komutu çalıştırın:

    `Remove-PSSession $Session` 



