---
title: Microsoft 365 grubu olarak gönder
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872270"
---
# <a name="send-as-microsoft-365-group"></a>Microsoft 365 grubu olarak gönder

Belirli kullanıcıların iletileri Microsoft 365 grubu olarak göndermesini sağlamak için farklı Gönder izinleri atayabilirsiniz:  

1. Exchange Online PowerShell 'e bağlanın.  

2. Aşağıdaki komutu çalıştırın:  

    Add-RecipientPermission `<GroupName>` -yönetici `<MailboxName>` -AccessRights SendAs

Daha fazla bilgi için, [Grup adına üyelerin adına veya göndermesine Izin ver](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)bölümüne bakın.