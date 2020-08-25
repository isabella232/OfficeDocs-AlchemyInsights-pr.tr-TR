---
title: Gönderen, Microsoft 365 grubuna gönderilen e-postayı almıyor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872268"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="a77df-102">Gönderen, Microsoft 365 grubuna gönderilen e-postayı almıyor</span><span class="sxs-lookup"><span data-stu-id="a77df-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="a77df-103">Varsayılan olarak, e-posta iletisinin göndereni Microsoft 365 grubuna, gönderen grubun bir üyesi olsa bile iletinin bir kopyasını gelen kutularına almaz.</span><span class="sxs-lookup"><span data-stu-id="a77df-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="a77df-104">Gönderenin, Microsoft 365 grubuna gönderdikleri her e-postanın bir kopyasını almasını sağlamak için bu EXO PowerShell komutunu kullanın:</span><span class="sxs-lookup"><span data-stu-id="a77df-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="a77df-105">Tüm posta kutularının ayarlarını aynı anda etkinleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="a77df-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="a77df-106">**Not** Bu ayarda yapılan değişikliklerin etkinleşmesi için bir saate kadar sürer.</span><span class="sxs-lookup"><span data-stu-id="a77df-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>