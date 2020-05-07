---
title: Exchange PowerShell ve temel kimlik doğrulamasının kullanımdan kaldırılması
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015709"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell ve temel kimlik doğrulamasının kullanımdan kaldırılması

Temel kimlik doğrulaması olmadan Exchange Online PowerShell'e bağlanma hakkında en son bilgiler için [lütfen bu sayfaya gidin](https://aka.ms/psbasicauth).

İstemci makinenizde Temel Kimlik Doğrulaması’nın yine de etkinleştirilmesi gerektiğini unutmayın.
Yeni PowerShell V2 modülü tüm REST tabanlı V2 Cmdlet’lerini etkinleştirmek için bağlantı kurarken Modern Kimlik Doğrulaması kullanır. V2 cmdlet’lerinin yanı sıra, Uzak PowerShell oturumu kurulmasını gerektiren eski Uzak PowerShell (RPS) Cmdlet’lerine de erişmenize olanak tanır. Modül hizmette kimlik doğrulaması yaparken Modern Kimlik Doğrulaması mekanizmasını kullansa bile, Windows makinesinde RPS oturumu oluşturmak için istemci makinesinde WinRM Temel Kimlik Doğrulaması’nın etkinleştirilmesi gerekir. Modern Kimlik Doğrulaması belirteçlerini aktarmak için WinRM Temel Kimlik Doğrulaması işlem hattı kullanılır. İstemci makinesinde WinRM Temel Kimlik Doğrulaması devre dışı bırakılırsa yeni V2 cmdlet’leri çalışmaya devam eder (ama eski RPS cmdlet’leri çalışmaz).
