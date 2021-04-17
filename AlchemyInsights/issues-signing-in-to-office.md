---
title: Microsoft 365 uygulamalarına oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833059"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Microsoft 365 uygulamalarında boş oturum açma ekranı

Bu sorunu çözmek için şunları deneyin:
- Windows ve Office için en [son güncelleştirmeleri](https://support.microsoft.com/help/4027667/windows-10-update) [yükleyin.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Internet Explorer seçeneklerini sıfırlama: Araçlar Internet Seçenekleri Gelişmiş Internet Explorer Ayarlarını Sıfırla 'ya gidin (özel ayarları kaybedeceğinizi unutmayın) ve Office'te oturum  >    >    >   açmayı yeniden deneyin.
- Windows Defender Application Guard'ı (WDAG) veya benzer güvenlik duvarını veya virüsten koruma programını devre dışı bırakma:
    1. Denetim Masası'nda **Programlar'a gidin** ve Windows özelliklerini **aç veya kapat'ı seçin.**
    2. Windows Defender Application Guard etkinleştirildiyse, bu özelliği devre dışı bırakmayı deneyin.<br/>
    **Not:** Bilgisayarı yeniden başlatmanız gerekiyor olabilir.
- Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) eklentisinin herhangi bir uygulama veya güvenlik duvarı/virüsten koruma programı tarafından engelli olmadığını kontrol edin.
- Windows [Kimlik Bilgileri Yöneticisi'ni](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) kullanarak Office kimlik bilgilerini temizleme.<br/>
    **Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değişti. (Örneğin: \Software\Microsoft\Office\16.0\Common\Identity\)

Daha fazla bilgi için [bkz. Windows 10 üzerinde Office 2016 derleme 16.0.7967'ye](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)güncelleştirdikten sonra oturum açma işlemiyle ilgili bağlantı sorunları.