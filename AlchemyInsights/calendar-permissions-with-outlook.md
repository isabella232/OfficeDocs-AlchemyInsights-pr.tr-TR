---
title: Takvim Izinleri
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748813"
---
# <a name="calendar-permissions"></a><span data-ttu-id="ad3c2-102">Takvim Izinleri</span><span class="sxs-lookup"><span data-stu-id="ad3c2-102">Calendar Permissions</span></span>

<span data-ttu-id="ad3c2-103">Kullanıcılar kendi takvim Izinlerini Web üzerinde veya başka istemcilerde Outlook 'ta değiştirebilir, ancak bir yönetici olarak araştırmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="ad3c2-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="ad3c2-104">Exchange PowerShell cmdlet 'i ile kullanıcının takviminde izin gösterilir:</span><span class="sxs-lookup"><span data-stu-id="ad3c2-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="ad3c2-105">Daha fazla bilgi görmek için aşağıdakilere bakın:</span><span class="sxs-lookup"><span data-stu-id="ad3c2-105">To see more information see the following:</span></span>

- [<span data-ttu-id="ad3c2-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="ad3c2-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="ad3c2-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="ad3c2-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="ad3c2-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="ad3c2-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="ad3c2-109">Takvim Izinlerinde Takvim paylaşımı 'nda kullanılır, Outlook takvimini paylaşma hakkında daha fazla bilgi için şu makalelere bakın:</span><span class="sxs-lookup"><span data-stu-id="ad3c2-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="ad3c2-110">Outlook takvimini başkalarıyla paylaşma</span><span class="sxs-lookup"><span data-stu-id="ad3c2-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="ad3c2-111">İş için Web üzerinde Outlook 'ta Takviminizi paylaşma</span><span class="sxs-lookup"><span data-stu-id="ad3c2-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="ad3c2-112">Takvim Izniyle ilgili sorunları gidermek için [destek ve Kurtarma Yardımcısı](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) aracını kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ad3c2-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>