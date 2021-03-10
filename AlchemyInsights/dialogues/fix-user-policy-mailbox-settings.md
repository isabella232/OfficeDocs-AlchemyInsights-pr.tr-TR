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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695898"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="a0b40-102">Kullanıcı ilkesi/posta kutusu ayarlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="a0b40-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="a0b40-103">Posta kutusunun gereksiz posta ayarları bu iletiyi etkiliyor.</span><span class="sxs-lookup"><span data-stu-id="a0b40-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="a0b40-104">Ayarları gözden geçirmek için şunları yapın:</span><span class="sxs-lookup"><span data-stu-id="a0b40-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="a0b40-105">Exchange Yönetim Kabuğu'nu başlatma.</span><span class="sxs-lookup"><span data-stu-id="a0b40-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="a0b40-106">Daha fazla bilgi için [bkz. Exchange Yönetim Kabuğu'nu açma.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="a0b40-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="a0b40-107">Bu komutu çalıştırın (kullanıcının e-posta adresini kullanarak):  **get-mailboxjokmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="a0b40-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="a0b40-108">Gönderenin e-posta adresinin **TrustedSendersAndDomains** veya **BlockedSendersAndDomains'in** bir parçası olup olduğunu kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="a0b40-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="a0b40-109">E-posta adresi listelerden birsinde yer alan bir adresse, bu adresi kaldırmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="a0b40-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="a0b40-110">Daha fazla bilgi edinmek için bkz. [Set-MailboxJokEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)</span><span class="sxs-lookup"><span data-stu-id="a0b40-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
