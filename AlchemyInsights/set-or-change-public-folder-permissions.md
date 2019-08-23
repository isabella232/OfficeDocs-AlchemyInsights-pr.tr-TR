---
title: Ayarlama veya ortak klasör izinlerini değiştirme
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
ms.openlocfilehash: 3f891beeba8303b05d6730f608034e22b2bcdb92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36550175"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="4b8c6-102">İzinler ve ortak klasörler</span><span class="sxs-lookup"><span data-stu-id="4b8c6-102">Permissions and Public Folders</span></span>

<span data-ttu-id="4b8c6-103">Ortak, Outlook, Exchange Yönetim Merkezi (TZT) kullanarak klasör izinlerini değiştirebilirsiniz veya PowerShell:</span><span class="sxs-lookup"><span data-stu-id="4b8c6-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="4b8c6-104">Outlook ilgili yönergeler için [burayı tıklatın](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="4b8c6-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="4b8c6-105">TZT için yönergeler için [Bu makaleye](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) bakın.</span><span class="sxs-lookup"><span data-stu-id="4b8c6-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> <span data-ttu-id="4b8c6-106">' I için TZT gitmek için [burada](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4b8c6-106">You can click [here](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) to navigate to EAC.</span></span> 
    
- <span data-ttu-id="4b8c6-107">PowerShell için Ekle PublicFolderClientPermission komutunu kullanma hakkında yönergeler için [Bu makaleye](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) bakın.</span><span class="sxs-lookup"><span data-stu-id="4b8c6-107">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="4b8c6-108">Bağlanmak için Exchange Powershell için yönergeler gereksinim duyarsanız, tıklatın [burada](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="4b8c6-108">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="4b8c6-109">**Harici kullanıcılar etkin posta ortak klasöre e-posta gönderemezsiniz**, neden olabilir, ortak klasörde izinleri yok dış e-posta teslimi için gerekli.</span><span class="sxs-lookup"><span data-stu-id="4b8c6-109">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="4b8c6-110">Bu Outlook yönergeleri kullanarak düzeltme [burada](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)veya PowerShell yönergeleri [burada](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="4b8c6-110">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

