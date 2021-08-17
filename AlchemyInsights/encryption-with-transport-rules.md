---
title: Aktarım kurallarıyla şifreleme
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079470"
---
# <a name="encryption-with-transport-rules"></a>Aktarım kurallarıyla şifreleme

[Exchange Yönetim Merkezi](https://go.microsoft.com/fwlink/p/?linkid=834822)’nde (EAC), ileti şifrelemesini tetiklemek için posta akışı kurallarınızda Office İleti Şifreleme (OME) özelliklerini kullanabilirsiniz. Aktarım Kuralı koşulunda **Office 365 İleti Şifrelemesi'ni ve hak korumasını uygula** seçeneğini belirtin.

- Daha fazla bilgi için bkz. [Şifreleme için Posta akışı kuralını tanımlama](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Powershell’de [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet’ini kullanın ve *ApplyOME* parametresini $true olarak ayarlayın.
