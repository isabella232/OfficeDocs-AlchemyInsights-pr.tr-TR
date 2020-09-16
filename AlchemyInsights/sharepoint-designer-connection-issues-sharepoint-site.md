---
title: SharePoint Designer bağlantı sorunları
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727191"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer bağlantı sorunları 

SharePoint Designer 'ın SharePoint sitelerinde bağlantı sorunları yaşıyorsanız, lütfen aşağıdaki ortak çözümleri deneyin.

Adım 1: SharePoint Designer 2013 SharePoint Designer [Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ve [SharePoint Designer 2013 için 2 Ağustos 2016 güncelleştirmesi](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)ile güncelleştirilmiştir.



Adım 2: yerel önbellek dosyalarını temizleyin:

1. SharePoint Designer 2013 'i kapatın.

2. Yerel bilgisayarda, aşağıdaki klasörlerden her birinde bulunan tüm dosyaları kaldırın.

    - %APPDATA%\Microsoft\Web sunucusu Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\appdata\local\microsoft\websitecache

3. SharePoint Designer 2013 açın ve çalışıp çalışmadığını görmek için hesabı yeniden girin.

Adım 3: [Windows cihazlarında Office 2013 Için modern kimlik doğrulamasını etkinleştirin](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Adım 4: yöneticilerin SharePoint Designer bağlantısına izin vermesi için SharePoint Yönetim Merkezi ayarlarındaki **özel komut dosyasına Izin vermesi** gerekir. Daha fazla [bilgi için bkz](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


