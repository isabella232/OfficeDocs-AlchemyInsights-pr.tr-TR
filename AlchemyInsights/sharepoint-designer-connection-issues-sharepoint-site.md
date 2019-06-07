---
title: Çevrimiçi SharePoint izin düzeylerini
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760712"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer bağlantı sorunları 

Lütfen SharePoint Designer SharePoint sitelerine bağlantı sorunlar yaşanıyorsa aşağıdaki ortak çözümleri deneyin.

Adım 1: Doğrulama SharePoint Designer güncelleştirilir.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [SharePoint Designer 2013 (KB3114721) güncelleştirmesi](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Adım 2: yerel önbellek dosyaları Temizle

- SharePoint Designer 2013 kapatın.

- Yerel bilgisayarda önbelleğe alınmış dosyaları silmek için aşağıdaki klasörleri bulun.

- Başlat, Çalıştır ve her biri altında bulunan tüm dosyaları sil konumları aşağıda.

%APPDATA%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

SharePoint Designer 2013 açın ve yeniden çalışıp çalışmadığını görmek için bir hesap girin.

Adım 3: [Modern Office 2013 aygıtlarda Windows kimlik doğrulamasını etkinleştirmek](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Adım 4: Yöneticiler SharePoint Designer bağlantıya izin veren özel komut dosyasına izin gerekir.

Ayrıntılı adımlar, örnekler ve dikkat edilmesi gereken noktalar için bkz: [izin ver veya özel komut dosyası engelleme](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


