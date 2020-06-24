---
title: Takvim İzinleri
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862164"
---
# <a name="calendar-permissions"></a>Takvim İzinleri

Kullanıcılar Web'de veya diğer istemcilerde Outlook ile kendi Takvim İzinlerini değiştirebilir, ancak yönetici olarak da araştırmanız gerekebilir.  
Exchange PowerShell cmdlet ile bir kullanıcının takviminde izin gösterecektir:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Daha fazla bilgi görmek için aşağıdakilere bakın:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Ekle-Posta KutusuFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Takvim İzinleri, Bir Outlook takvimini paylaşma hakkında daha fazla bilgi görmek için takvim lerin paylaşımında kullanılır, aşağıdaki makalelere bakın:

- [Outlook takvimini başkalarıyla paylaşma](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [İş için web'de takviminizi Outlook'ta paylaşın](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Takvim İzni'ni gidermek için [Destek ve Kurtarma Yardımcısı](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) aracını kullanabilirsiniz.