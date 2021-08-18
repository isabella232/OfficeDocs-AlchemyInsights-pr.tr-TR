---
title: ClientAccessServerEnabled'ı True olarak ayarlama
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320376"
---
# <a name="set-clientaccessserverenabled-to-true"></a>ClientAccessServerEnabled'ı True olarak ayarlama

Şifreli bir e-posta iletisini açasanız ve bunun yerine **bir rpmsg eki** görüyorsanız aşağıdaki adımları uygulayın:

1. Bağlan PowerShell Exchange Online e geri tarak.

    **Not:** Exchange Online PowerShell'e bağlanmak için genel yönetici veya yönetici hesabı Exchange oturum açın.

   a. Windows PowerShell'i açın ve sonra aşağıdaki komutu çalıştırın:`$UserCredential = Get-Credential`
   b. Oturum **Windows PowerShell İsteği iletişim** kutusuna iş veya okul hesabınızla parolanızı girin, c. **Tamam**'a tıklayın. 

2. Yeni bir oturum oluşturmak için aşağıdaki komutu çalıştırın:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Aşağıdaki komutu çalıştırın:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Çalıştır `Get-IRMConfiguration` komutu.

4. **ClientAccessServerEnabled ayarını** kontrol edin. 

    a. **ClientAccessServerEnabled ayarı** False olarak **ayarlanmışsa** aşağıdaki cmdlet'i çalıştırın:`Set-IRMConfiguration -ClientAccessServerEnabled $True`

**İpucu:** Her zaman aşağıdaki komutu kullanarak PowerShell oturumlarınızı kapatın: `Remove-PSSession $Session`

Daha fazla bilgi için [bkz. Exchange Online PowerShell..](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

