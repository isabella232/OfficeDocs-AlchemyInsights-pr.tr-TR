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
ms.openlocfilehash: 1868b8b04df012d44781f86ee75120ca443af5be5801074329f17c0e40a5acc7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060912"
---
# <a name="permissions-and-public-folders"></a>İzinler ve Ortak Klasörler

Ortak Klasörlerinizin izinlerini değiştirmek için Ortak Klasörler'i, Outlook merkezi (EAC) Exchange PowerShell'i kullanın:
  
- Daha Outlook için buraya [tıklayın.](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)
    
- EAC'de yönergeler için [bu makaleye](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) bakın. 
    
- Powershell'de Add-PublicFolderClientPermission [](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) commandlet'ini kullanma yönergeleri için bu Add-PublicFolderClientPermission bakın. Exchange Powershell'e bağlanma yönergelerine ihtiyacınız varsa, buraya [tıklayın.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)
    
Dış **kullanıcılar posta özellikli Ortak Klasöre e-posta** göndere iletileri göndereene kadar, bunun nedeni ortak klasörde dış e-posta teslimi için gereken izinlerin eksik olması olabilir. Bu sorunu, buradaki Outlook [veya](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)PowerShell yönergelerini kullanarak [düzeltabilirsiniz.](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)
  

