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
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994885"
---
# <a name="set-clientaccessserverenabled-to-true"></a>ClientAccessServerEnabled'ı True olarak ayarlama

Şifreli bir e-posta iletisini a açasanız ve bunun yerine **bir rpmsg eki** görüyorsanız aşağıdaki adımları uygulayın:

1. Bağlan PowerShell Exchange Online e geri tarak.

> [!NOTE]
> Exchange Online PowerShell'e bağlanmak için genel yönetici veya yönetici hesabı Exchange oturum açın.

   a. Windows PowerShell'i açın ve sonra aşağıdaki komutu çalıştırın:`$UserCredential = Get-Credential`
b. Kimlik **Windows PowerShell kutusuna iş** veya okul hesabınızla parolanızı girin, c. **Tamam**'a tıklayın. 

2. Yeni bir oturum oluşturmak için aşağıdaki komutu çalıştırın:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Aşağıdaki komutu çalıştırın:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Çalıştır `Get-IRMConfiguration` komutu.

4. **ClientAccessServerEnabled ayarını** kontrol edin. 

    a. **ClientAccessServerEnabled ayarı** False olarak **ayarlanmışsa** aşağıdaki cmdlet'i çalıştırın:`Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Her zaman aşağıdaki komutu kullanarak PowerShell oturumlarınızı kapatın: `Remove-PSSession $Session`

Daha fazla bilgi için [bkz. Exchange Online PowerShell..](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

