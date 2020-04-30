---
title: Aktarım kurallarıyla şifreleme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915285"
---
# <a name="encryption-with-transport-rules"></a>Aktarım kurallarıyla şifreleme

[Exchange Yönetim Merkezi](https://go.microsoft.com/fwlink/p/?linkid=834822)’nde (EAC), ileti şifrelemesini tetiklemek için posta akışı kurallarınızda Office İleti Şifreleme (OME) özelliklerini kullanabilirsiniz. Aktarım Kuralı koşulunda **Office 365 İleti Şifrelemesi'ni ve hak korumasını uygula** seçeneğini belirtin.

- Daha fazla bilgi için bkz. [Şifreleme için Posta akışı kuralını tanımlama](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Powershell’de [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet’ini kullanın ve *ApplyOME* parametresini $true olarak ayarlayın.
