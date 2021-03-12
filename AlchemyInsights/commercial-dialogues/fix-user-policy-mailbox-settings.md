---
title: Kullanıcı ilkesi/posta kutusu ayarlarını düzeltme
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750566"
---
# <a name="fix-user-policymailbox-settings"></a>Kullanıcı ilkesi/posta kutusu ayarlarını düzeltme

Posta kutusunun gereksiz posta ayarları bu iletiyi etkiliyor. Ayarları gözden geçirmek için şunları yapın:

1. Exchange Yönetim Kabuğu'nu başlatma. Daha fazla bilgi için [bkz. Exchange Yönetim Kabuğu'nu açma.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Bu komutu çalıştırın (kullanıcının e-posta adresini kullanarak):  **get-mailboxjokmailconfiguration -identity "user@domain.com"**
3. Gönderenin e-posta adresinin **TrustedSendersAndDomains** veya **BlockedSendersAndDomains'in** bir parçası olup olduğunu kontrol edin. E-posta adresi listelerden birsinde yer alan bir adresse, bu adresi kaldırmanız gerekir. Daha fazla bilgi edinmek için bkz. [Set-MailboxJokEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
