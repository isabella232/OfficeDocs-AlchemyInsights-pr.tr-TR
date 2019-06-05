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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716911"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer bağlantı sorunları 

<p>Lütfen SharePoint Designer SharePoint sitelerine bağlantı sorunlar yaşanıyorsa aşağıdaki ortak çözümleri deneyin.</p> <p><strong>Adım 1:</strong> <strong>Doğrulamak SharePoint Designer güncelleştirilir&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">SharePoint Designer 2013 (KB3114721) güncelleştirmesi</a></li> </ul> <p><strong>Adım 2:</strong> <strong>Yerel önbellek dosyaları Temizle</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">SharePoint Designer 2013 kapatın.&nbsp;</li> <li style="font-weight: 400;">Yerel bilgisayarda önbelleğe alınmış dosyaları silmek için aşağıdaki klasörleri bulun.&nbsp;</li> <li style="font-weight: 400;">' I <strong>Start -&gt; çalıştırmak</strong> ve her biri altında bulunan tüm dosyaları silin konumları aşağıda.&nbsp;<br /><br />%APPDATA%\Microsoft\Web server Extensions\Cache<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">SharePoint Designer 2013 açın ve yeniden çalışıp çalışmadığını görmek için bir hesap girin.</li> </ol> <p><strong>Adım 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Modern Office 2013 aygıtlarda Windows kimlik doğrulamasını etkinleştirmek</strong></a>&nbsp;</p> <p><strong>Adım 4:</strong> <strong>Yöneticiler izin özel SharePoint Designer bağlantıya izin vermek için komut dosyası gerekir</strong>.</p> <p>Ayrıntılı adımlar, örnekler ve dikkat edilmesi gereken noktalar için bkz: <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">izin ver veya özel komut dosyası engelleme</a>.&nbsp;</p>


