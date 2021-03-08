---
title: Microsoft 365 grubuna gönderilen iletiler tüm üyeler tarafından alınmıyor
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 080c060f5675065704c7209bd15e4cbb1236b8db
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480703"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="0ff57-102">Bir Microsoft 365 grubuna gönderilen iletiler tüm üyeler tarafından alınmıyor</span><span class="sxs-lookup"><span data-stu-id="0ff57-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="0ff57-103">Tüm grup üyelerinin e-posta almak üzere abone olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="0ff57-103">Ensure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="0ff57-104">[Outlook’ta bir grubu takip etme](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36) makalesine bakın.</span><span class="sxs-lookup"><span data-stu-id="0ff57-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="0ff57-105">Grup e-postalarına abone olmuş üyelerin ileti durumunu kontrol etmek için aşağıdaki komutu [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)’de çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="0ff57-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

<span data-ttu-id="0ff57-106">Tüm grup üyelerini Microsoft 365 grubuna gönderilen e-postaları kendi gelen kutularında alacak şekilde yapılandırmak için aşağıdaki EXO PowerShell komutunu kullanın:</span><span class="sxs-lookup"><span data-stu-id="0ff57-106">Use the following EXO PowerShell command to configure all group members to receive emails sent to Microsoft 365 group in their inbox:</span></span>

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

<span data-ttu-id="0ff57-107">Örneğin:</span><span class="sxs-lookup"><span data-stu-id="0ff57-107">For example:</span></span>

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`