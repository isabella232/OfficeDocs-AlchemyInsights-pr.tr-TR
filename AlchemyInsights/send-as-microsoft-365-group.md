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
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="d724e-102">Microsoft 365 grubu olarak gönder</span><span class="sxs-lookup"><span data-stu-id="d724e-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="d724e-103">Belirli kullanıcıların iletileri Microsoft 365 grubu olarak göndermesini sağlamak için farklı Gönder izinleri atayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="d724e-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="d724e-104">Exchange Online PowerShell 'e bağlanın.</span><span class="sxs-lookup"><span data-stu-id="d724e-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="d724e-105">Aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="d724e-105">Run the following command:</span></span>  

    <span data-ttu-id="d724e-106">Add-RecipientPermission `<GroupName>` -yönetici `<MailboxName>` -AccessRights SendAs</span><span class="sxs-lookup"><span data-stu-id="d724e-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="d724e-107">Daha fazla bilgi için, [Grup adına üyelerin adına veya göndermesine Izin ver](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="d724e-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>