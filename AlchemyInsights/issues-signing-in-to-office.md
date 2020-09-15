---
title: Microsoft 365 uygulamalarında oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695307"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Microsoft 365 uygulamalarında boş oturum açma ekranı

Bu sorunu çözmek için aşağıdakileri deneyin:
- En son [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ve [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)güncelleştirmelerini yükleyin.
- Internet Explorer seçeneklerini sıfırlayın: araçlara gidin **Tools**  >  **İnternet seçenekleri**  >  **Gelişmiş**  >  **Internet Explorer ayarlarını sıfırlayın** (özel ayarları kaybedeceğinizi unutmayın) ve ardından Office 'te yeniden oturum açmayı deneyin.
- Windows Defender Application Guard (WDAG) veya benzer bir güvenlik duvarını veya antivirüs programını devre dışı bırakın:
    1. Denetim Masası 'nda, **Programlar**'a gidin ve **Windows özelliklerini aç veya kapat**'ı seçin.
    2. Windows Defender Application Guard etkinse, devre dışı bırakmayı deneyin.<br/>
    **Not:** Bilgisayarı yeniden başlatmanız gerekebilir.
- Microsoft. AAD. BrokerPlugin [AAD WAM eklentisinin](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) herhangi bir uygulama veya güvenlik duvarı/virüs önleme programı tarafından engellenmediğinden emin olun.
- Windows kimlik bilgileri Yöneticisi 'Ni kullanarak [Office kimlik bilgilerini temizleyin](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .<br/>
    **Not:** Office 2016 için kayıt defteri yolları 16,0 olarak değiştirilmiştir. (Örn: \Software\Microsoft\Office\16.0\Common\Identity\)

Daha fazla bilgi için, [Windows 10 ' da Office 2016 derleme 16.0.7967 güncelleştirmeden sonra oturum açma 'Daki bağlantı sorunlarını](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)izleyin.