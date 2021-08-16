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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034738"
---
# <a name="fix-user-policymailbox-settings"></a>Kullanıcı ilkesi/posta kutusu ayarlarını düzeltme

Posta kutusunda gereksiz posta ayarları bu iletiyi etkiliyordur. Ayarları gözden geçirmek için şunları yapın:

1. Yönetim Exchange'i başlatma. Daha fazla bilgi için [bkz. Exchange Kabuğu'nu açma.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Bu komutu çalıştırın (kullanıcının e-posta adresini kullanarak):  **get-mailboxmailconfiguration -identity "user@domain.com"**
3. Gönderenin e-posta adresinin **TrustedSendersAndDomains** veya **BlockedSendersAndDomains kapsamında olupdiğini kontrol edin.** E-posta adresi listelerden birsinde yer alan bir adresse, bu adresi kaldırmanız gerekir. Daha fazla bilgi edinmek için bkz. [Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
