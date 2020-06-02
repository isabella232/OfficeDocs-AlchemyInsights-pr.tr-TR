---
title: SharePoint Designer bağlantı sorunları
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511564"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer bağlantı sorunları 

SharePoint Designer SharePoint sitelerine bağlantı sorunları yaşıyorsa, lütfen aşağıdaki ortak çözümleri deneyin.

Adım 1: SharePoint Designer 2013'ün [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ve [SharePoint Designer 2013 için 2 Ağustos 2016 Güncelleştirmesi](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)ile güncelleştirin.



Adım 2: Yerel önbellek dosyalarını temizleyin:

1. SharePoint Designer 2013'u kapatın.

2. Yerel bilgisayarda, aşağıdaki klasörlerin her birinde bulunan tüm dosyaları kaldırın.

    - %APPDATA%\Microsoft\Web Sunucusu Uzantıları\Önbellek
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyÖnbellek
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteÖnbellek

3. SharePoint Designer 2013'u açın ve çalışıp çalışmadığına görmek için hesabı yeniden girin.

Adım 3: [Windows Aygıtlarında Office 2013 için Modern Kimlik Doğrulamayı Etkinleştirin.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Adım 4: Yöneticilerin SharePoint Designer bağlantısına izin vermek için SharePoint Yönetici Merkezi ayarlarında **Özel Komut Dosyasına İzin** Vermeleri Gerekir. Bkz. Daha fazla bilgi için [özel komut dosyasına izin ver veya engelleyin.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


