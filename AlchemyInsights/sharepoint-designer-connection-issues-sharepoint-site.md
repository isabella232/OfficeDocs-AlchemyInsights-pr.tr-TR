---
title: SharePoint Designer bağlantı sorunları
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508443"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer bağlantı sorunları 

SharePoint Designer SharePoint sitelerine bağlantı sorunları yaşıyor, lütfen aşağıdaki ortak çözümleri deneyin.

1. adım: SharePoint Designer 2013 [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ve [2 Ağustos 2016 için SharePoint Designer 2013 güncelleştirme](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)güncelleştirilmiş olduğunu doğrulamak.



Adım 2: yerel önbellek dosyaları temizleyin:

1. SharePoint Designer 2013 kapatın.

2. Yerel bilgisayarda, her biri aşağıdaki klasörler içinde bulunan tüm dosyaları kaldırın.

    - %APPDATA%\Microsoft\Web server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. SharePoint Designer 2013 açın ve yeniden çalışıp çalışmadığını görmek için bir hesap girin.

Adım 3: [Windows cihazlarda Office 2013 için Modern kimlik doğrulamasını etkinleştirin](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Adım 4: Yöneticiler **Özel komut dosyası izin vermek** için SharePoint Yönetim Merkezi ayarlarını SharePoint Designer bağlantıya izin vermek için gerekir. Bkz: [izin ver veya özel komut dosyası engelleme](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) daha fazla bilgi için.


