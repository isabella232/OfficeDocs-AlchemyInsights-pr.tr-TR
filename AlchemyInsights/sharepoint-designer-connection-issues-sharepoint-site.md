---
title: SharePoint Tasarımcı bağlantı sorunları
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942045"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Tasarımcı bağlantı sorunları 

Tasarımcı SharePoint site sitelerine bağlantı sorunları SharePoint, lütfen aşağıdaki yaygın çözümleri deneyin.

1. Adım: SharePoint Designer 2013'SharePoint [Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ve SharePoint Designer [2013 için 2 Ağustos 2016 Güncelleştirmesi](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)ile güncelleştirilmiş olduğunu doğrulayın.



2. Adım: Yerel önbellek dosyalarını temizleyin:

1. Tasarım SharePoint 2013'ü kapatın.

2. Yerel bilgisayarda, aşağıdaki klasörlerin her birsinde bulunan tüm dosyaları kaldırın.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. SharePoint Designer 2013'ü açın ve işe yarar mı diye görmek için hesabı yeniden girin.

3. Adım: [Mobil Cihazlarda Office 2013](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)için Modern kimlik Windows etkinleştirin.

4. Adım: Yöneticilerin  Tasarımcı bağlantısına izin vermek için SharePoint Merkezi ayarlarında Özel Betiklere İzin SharePoint gerekir. Daha [fazla bilgi için bkz. Özel betiklere izin verme](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) veya bunu engelleme.


