---
title: Takvim Izinleri
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
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748813"
---
# <a name="calendar-permissions"></a>Takvim Izinleri

Kullanıcılar kendi takvim Izinlerini Web üzerinde veya başka istemcilerde Outlook 'ta değiştirebilir, ancak bir yönetici olarak araştırmanız gerekebilir.  
Exchange PowerShell cmdlet 'i ile kullanıcının takviminde izin gösterilir:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Daha fazla bilgi görmek için aşağıdakilere bakın:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Takvim Izinlerinde Takvim paylaşımı 'nda kullanılır, Outlook takvimini paylaşma hakkında daha fazla bilgi için şu makalelere bakın:

- [Outlook takvimini başkalarıyla paylaşma](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [İş için Web üzerinde Outlook 'ta Takviminizi paylaşma](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Takvim Izniyle ilgili sorunları gidermek için [destek ve Kurtarma Yardımcısı](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) aracını kullanabilirsiniz.