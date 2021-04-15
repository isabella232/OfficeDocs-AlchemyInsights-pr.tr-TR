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
# <a name="permissions-and-public-folders"></a>İzinler ve Ortak Klasörler

Ortak Klasörlerinizin izinlerini Outlook, Exchange admin center (EAC) veya PowerShell kullanarak değiştirebilirsiniz:
  
- Outlook yönergeleri için buraya [tıklayın.](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)
    
- EAC'de yönergeler için [bu makaleye](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) bakın. 
    
- Powershell'de Add-PublicFolderClientPermission [](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) commandlet'ini kullanma yönergeleri için bu Add-PublicFolderClientPermission bakın. Exchange Powershell'e bağlanma yönergelerine ihtiyacınız varsa, buraya [tıklayın.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)
    
Dış **kullanıcılar posta özellikli Ortak Klasöre e-posta** göndere iletileri göndereene kadar, bunun nedeni ortak klasörde dış e-posta teslimi için gereken izinlerin eksik olması olabilir. Buradaki Outlook yönergelerini veya [buradaki](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)PowerShell yönergelerini kullanarak bu durumu [düzeltebilirsiniz.](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)
  

