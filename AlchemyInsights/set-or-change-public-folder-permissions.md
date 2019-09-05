---
title: Ortak klasör izinlerini ayarlama veya değiştirme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 1015c2203406e15d6b418c387b6632a182d6d2ff
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36734689"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="03077-102">İzinler ve Ortak Klasörler</span><span class="sxs-lookup"><span data-stu-id="03077-102">Permissions and Public Folders</span></span>

<span data-ttu-id="03077-103">Outlook, Exchange yönetici merkezi (EAC) veya PowerShell'i kullanarak Ortak Klasörlerinizdeki izinleri değiştirebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="03077-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="03077-104">Outlook yönergeleri için [burayı tıklatın.](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)</span><span class="sxs-lookup"><span data-stu-id="03077-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="03077-105">EAC için, talimatlar için [bu makaleye](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) bakın.</span><span class="sxs-lookup"><span data-stu-id="03077-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="03077-106">Powershell için, Ekle-PublicFolderClientPermission komut unu kullanma yönergeleri için [bu makaleye](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) bakın.</span><span class="sxs-lookup"><span data-stu-id="03077-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="03077-107">Exchange Powershell'e bağlanmak için talimatlara ihtiyacınız varsa, [buraya](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)tıklayın.</span><span class="sxs-lookup"><span data-stu-id="03077-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="03077-108">**Harici kullanıcılar posta yla etkinleştirilmiş genel klasöre e-posta gönderemiyorsa,** bunun nedeni ortak klasörün harici e-posta teslimi için gereken izinleri eksik olması olabilir.</span><span class="sxs-lookup"><span data-stu-id="03077-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="03077-109">Bunu [outlook](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)yönergelerini kullanarak veya [powershell yönergelerini buradan](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)düzeltebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="03077-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

