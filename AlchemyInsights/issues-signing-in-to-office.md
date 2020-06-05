---
title: Microsoft 365 uygulamalarında oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579921"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Microsoft 365 uygulamalarında boş oturum açma ekranı

Bu sorunu gidermek için aşağıdakileri deneyin:
- [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ve [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)için en son güncelleştirmeleri yükleyin.
- Internet Explorer seçeneklerini sıfırla: **Araçlar**  >  **Internet Seçenekleri**  >  **Gelişmiş**Sıfırlama Internet  >  **Explorer Ayarlarını** (özel ayarları kaybedeceğinizi unutmayın) gidin ve ardından Office'te yeniden oturum açmayı deneyin.
- Windows Defender Application Guard (WDAG) veya benzer bir güvenlik duvarı veya anti-virüs programı devre dışı:
    1. Denetim Masası'nda **Programlar'a**gidin ve ardından **Windows özelliklerini açıp kapatmayı**seçin.
    2. Windows Defender Application Guard etkinse, devre dışı bırakmayı deneyin.<br/>
    **Not:** Bilgisayarı yeniden başlatmanız gerekebilir.
- Microsoft.AAD.BrokerPlugin [AAD WAM eklentisinin](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) herhangi bir uygulama veya güvenlik duvarı/virüsten koruma programı tarafından engellenmediğinden emin olun.
- Windows Kimlik Bilgileri Yöneticisi'ni kullanarak [Office kimlik bilgilerini temizleyin.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)<br/>
    **Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değiştirildi. (Ör. \Software\Microsoft\Office\16.0\Common\Identity\)

Daha fazla bilgi için bkz: [Windows 10'da Office 2016'da 16.0.7967'yi oluştur'a güncellemeden sonra oturum açma](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)bağlantısı sorunları.