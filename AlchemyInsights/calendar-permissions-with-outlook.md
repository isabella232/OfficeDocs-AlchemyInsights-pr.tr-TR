---
title: Takvim İzinleri
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
- "3800009"
- "611"
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046124"
---
# <a name="calendar-permissions"></a>Takvim İzinleri

Kullanıcılar Web'deki veya diğer istemcilerde Outlook izinleriyle kendi Takvim İzinlerini değiştirebilir, ancak bir yönetici olarak sizin de araştırmanız gerekir.  
PowerShell Exchange cmdlet'i kullanıcının takviminde izin gösterir:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Daha fazla bilgi için aşağıdakilere bakın:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Takvim İzinleri takvimlerin paylaşımında kullanılır; takvim paylaşımı hakkında daha fazla bilgi Outlook için şu makalelere bakın:

- [Outlook takvimini başkalarıyla paylaşma](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Web üzerinde Outlook İş'te takviminizi paylaşma](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Takvim İzni sorunlarını gidermek için Takvim izni [Destek ve Kurtarma Yardımcısı](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) kullanabilirsiniz.