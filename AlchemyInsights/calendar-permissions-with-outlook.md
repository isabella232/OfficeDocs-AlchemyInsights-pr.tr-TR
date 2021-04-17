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
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819928"
---
# <a name="calendar-permissions"></a>Takvim İzinleri

Kullanıcılar Web üzerinde Outlook'la veya diğer istemcilerle kendi Takvim İzinlerini değiştirebilir, ancak bir yönetici olarak sizin de araştırmanız gerekir.  
Exchange PowerShell cmdlet'iyle kullanıcının takviminde izinler size gösterir:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Daha fazla bilgi için aşağıdakilere bakın:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Takvim İzinleri takvimlerin paylaşımında kullanılır; Outlook takvimini paylaşma hakkında daha fazla bilgi için şu makalelere bakın:

- [Outlook takvimini başkalarıyla paylaşma](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Web üzerinde Outlook İş'te takviminizi paylaşma](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Takvim İzni sorunlarını gidermek için Destek ve [Kurtarma Yardımcısı aracını kullanabilirsiniz.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)