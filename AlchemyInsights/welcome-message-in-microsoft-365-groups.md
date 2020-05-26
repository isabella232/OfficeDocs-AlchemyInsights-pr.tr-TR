---
title: Microsoft 365 Gruplarında hoş geldiniz iletisi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358334"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Microsoft 365 Gruplarında hoş geldiniz iletisi

"UnifiedGroupWelcomeMessageEnabled" özelliği Doğruysa, Microsoft 365 grubuna katılan yeni kullanıcılar hoş geldiniz e-postası alır.

Karşılama iletisini devre dışı kullanabilirsiniz, aşağıdaki [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) komutunu kullanın:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
