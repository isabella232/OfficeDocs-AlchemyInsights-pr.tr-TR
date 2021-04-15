---
title: Ortak klasör izinlerini ayarlama veya değiştirme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: e419c72a890e68fc7b6d40d2b64406e42f9b0769
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51789227"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="86c10-102">İzinler ve Ortak Klasörler</span><span class="sxs-lookup"><span data-stu-id="86c10-102">Permissions and Public Folders</span></span>

<span data-ttu-id="86c10-103">Ortak Klasörlerinizin izinlerini Outlook, Exchange admin center (EAC) veya PowerShell kullanarak değiştirebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="86c10-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="86c10-104">Outlook yönergeleri için buraya [tıklayın.](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)</span><span class="sxs-lookup"><span data-stu-id="86c10-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="86c10-105">EAC'de yönergeler için [bu makaleye](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) bakın.</span><span class="sxs-lookup"><span data-stu-id="86c10-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="86c10-106">Powershell'de Add-PublicFolderClientPermission [](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) commandlet'ini kullanma yönergeleri için bu Add-PublicFolderClientPermission bakın.</span><span class="sxs-lookup"><span data-stu-id="86c10-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="86c10-107">Exchange Powershell'e bağlanma yönergelerine ihtiyacınız varsa, buraya [tıklayın.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)</span><span class="sxs-lookup"><span data-stu-id="86c10-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="86c10-108">Dış **kullanıcılar posta özellikli Ortak Klasöre e-posta** göndere iletileri göndereene kadar, bunun nedeni ortak klasörde dış e-posta teslimi için gereken izinlerin eksik olması olabilir.</span><span class="sxs-lookup"><span data-stu-id="86c10-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="86c10-109">Buradaki Outlook yönergelerini veya [buradaki](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)PowerShell yönergelerini kullanarak bu durumu [düzeltebilirsiniz.](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)</span><span class="sxs-lookup"><span data-stu-id="86c10-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

