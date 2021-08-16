---
title: Exchange PowerShell ve temel kimlik doğrulamasının kullanımdan kaldırılması
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
- "3500011"
- "4577"
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069264"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell ve temel kimlik doğrulamasının kullanımdan kaldırılması

Temel kimlik doğrulaması olmadan Exchange Online PowerShell'e bağlanma hakkında en son bilgiler için [lütfen bu sayfaya gidin](https://aka.ms/exops-docs). PowerShell V2 modülü temel kimlik doğrulamasını kullanmaz.

İstemci makinenizde Temel Kimlik Doğrulaması’nın yine de etkinleştirilmesi gerektiğini unutmayın.
Yeni PowerShell V2 modülü tüm REST tabanlı V2 Cmdlet’lerini etkinleştirmek için bağlantı kurarken Modern Kimlik Doğrulaması kullanır. V2 cmdlet’lerinin yanı sıra, Uzak PowerShell oturumu kurulmasını gerektiren eski Uzak PowerShell (RPS) Cmdlet’lerine de erişmenize olanak tanır. Modül hizmette kimlik doğrulaması yaparken Modern Kimlik Doğrulaması mekanizmasını kullansa bile, Windows makinesinde RPS oturumu oluşturmak için istemci makinesinde WinRM Temel Kimlik Doğrulaması’nın etkinleştirilmesi gerekir. Modern Kimlik Doğrulaması belirteçlerini aktarmak için WinRM Temel Kimlik Doğrulaması işlem hattı kullanılır. İstemci makinesinde WinRM Temel Kimlik Doğrulaması devre dışı bırakılırsa yeni V2 cmdlet’leri çalışmaya devam eder (ama eski RPS cmdlet’leri çalışmaz).
