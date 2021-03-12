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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749973"
---
# <a name="set-clientaccessserverenabled-to-true"></a>ClientAccessServerEnabled'ı True olarak ayarlama

Şifreli bir e-posta iletisini açasanız ve bunun yerine **bir rpmsg** eki görüyorsanız, aşağıdaki adımları uygulayın:

1. Exchange Online PowerShell'e bağlanın.

> [!NOTE]
> Exchange Online PowerShell'e bağlanmak için genel yönetici veya Exchange yönetici hesabıyla oturum açın.

   a. Windows PowerShell'i açın ve aşağıdaki komutu çalıştırın: `$UserCredential = Get-Credential`
b. Windows **PowerShell Kimlik Bilgileri İsteği** iletişim kutusuna iş veya okul hesabınızla parolanızı girin, c. **Tamam**'a tıklayın. 

2. Yeni bir oturum oluşturmak için aşağıdaki komutu çalıştırın:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Aşağıdaki komutu çalıştırın:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Çalıştır `Get-IRMConfiguration` komutu.

4. **ClientAccessServerEnabled ayarını** kontrol edin. 

    a. **ClientAccessServerEnabled** ayarı False olarak **ayarlanmışsa,** aşağıdaki cmdlet'i çalıştırın:`Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Her zaman aşağıdaki komutu kullanarak PowerShell oturumlarınızı kapatın: `Remove-PSSession $Session`

Daha fazla bilgi için [bkz. Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

